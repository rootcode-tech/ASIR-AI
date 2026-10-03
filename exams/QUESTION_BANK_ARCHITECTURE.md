# Arquitectura del banco de preguntas de ASIR-AI

**Versión:** 0.1.0  
**Estado:** aprobado para implementación

## 1. Objetivo

El banco de preguntas de ASIR-AI debe permitir construir exámenes reproducibles, auditables y equivalentes sin que una IA invente preguntas en tiempo de ejecución.

La regla principal es:

```text
la IA puede explicar
la IA puede ayudar a revisar
la IA puede analizar respuestas

pero

la IA no crea preguntas calificables durante un examen
```

Las preguntas calificables se redactan, revisan, versionan y aprueban previamente dentro del repositorio.

## 2. Fuente de verdad

La fuente de verdad del sistema de evaluación será el contenido versionado en Git.

Cada ítem debe tener:

- identificador estable;
- asignatura;
- UD;
- objetivo o competencia evaluada;
- nivel D1-D4;
- tipo de ítem;
- modalidad;
- tiempo estimado;
- enunciado;
- respuesta esperada o criterio de resolución;
- rúbrica o mecanismo de corrección;
- errores críticos cuando proceda;
- versión;
- estado editorial.

## 3. Identificadores

Formato base:

```text
ASIR-XX-UDYY-QZZZ
```

Ejemplo:

```text
ASIR-02-UD03-Q014
```

Significa:

- `ASIR-02`: asignatura;
- `UD03`: unidad didáctica;
- `Q014`: ítem número 14 de esa UD.

Un identificador no se reutiliza después de publicar un ítem.

Si una pregunta cambia de forma sustancial, se incrementa su versión. Si cambia la competencia evaluada o deja de ser equivalente, se crea un nuevo ID.

## 4. Estados editoriales

Cada pregunta tendrá uno de estos estados:

```text
draft
review
approved
retired
```

### draft

Pregunta en construcción. No puede aparecer en un examen calificable.

### review

Pregunta terminada pero pendiente de revisión académica o técnica.

### approved

Pregunta aprobada y disponible para exámenes.

### retired

Pregunta retirada. Se conserva por trazabilidad, pero no puede seleccionarse para nuevos exámenes.

## 5. Niveles de dificultad

Se utilizará la escala común de ASIR-AI:

- `D1` — reconocimiento y comprensión;
- `D2` — aplicación;
- `D3` — diagnóstico y análisis;
- `D4` — integración, diseño o decisión justificada.

La dificultad no se determina por lo largo que sea el enunciado, sino por la operación cognitiva que debe realizar el alumno.

## 6. Tipos de ítem

Valores iniciales:

```text
short_answer
multiple_choice
calculation
command_interpretation
log_analysis
configuration
sql
script
troubleshooting
architecture
comparison
case_study
practical_lab
oral
english
```

El catálogo podrá ampliarse, pero no deben crearse sinónimos innecesarios.

## 7. Modalidades

Cada ítem debe declarar su modalidad:

```text
closed_book
open_docs
open_lab
controlled_ai
```

Un examen puede mezclar modalidades por bloques, pero cada pregunta debe dejar claro qué recursos se permiten.

## 8. Uso de IA

Por defecto:

```yaml
ai:
  allowed: false
```

Cuando una competencia sea precisamente evaluar el uso crítico de IA:

```yaml
ai:
  allowed: true
  mode: controlled
  purpose: verification
```

En esos casos no se evalúa que la IA produzca una respuesta bonita. Se evalúa que el alumno sea capaz de:

1. formular correctamente el problema;
2. inspeccionar la respuesta;
3. detectar afirmaciones dudosas;
4. contrastarlas con documentación o evidencia;
5. corregir errores;
6. verificar el resultado real.

## 9. Pregunta, respuesta y rúbrica

Cada ítem calificable debe incluir internamente suficiente información para corregirlo sin depender de interpretación improvisada.

### Respuesta determinista

Cuando exista un resultado verificable, se prefiere corrección determinista.

Ejemplos:

- SQL: ejecutar y verificar resultado, estructura, restricciones o estado final;
- Linux: scripts que comprueban usuarios, grupos, permisos, servicios o archivos;
- Docker: inspeccionar contenedores, redes, volúmenes y health checks;
- Ansible: comprobar estado final e idempotencia;
- Terraform: validar configuración, plan y estado esperado;
- redes: comprobar direccionamiento, rutas, DNS, puertos y conectividad;
- aplicaciones web: health checks, códigos HTTP, TLS, persistencia y logs.

### Rúbrica

Cuando una respuesta admita varias soluciones correctas, debe existir una rúbrica.

La rúbrica debe valorar los aspectos pertinentes del marco común, por ejemplo:

- resultado correcto;
- procedimiento o razonamiento;
- verificación;
- seguridad, reversibilidad e impacto;
- claridad técnica.

## 10. Errores críticos

Los errores críticos no deben improvisarse durante la corrección.

Si una pregunta puede implicar un fallo grave, el propio ítem debe definirlo en `critical_errors`.

Ejemplos:

- pérdida evitable de datos;
- exposición de credenciales;
- permisos inseguros usados para forzar una solución;
- desactivar controles de seguridad sin justificación;
- acción destructiva sin backup o rollback cuando eran necesarios;
- afirmar recuperación sin haber validado el restore.

## 11. Variantes

Se permiten variantes predefinidas de un mismo patrón, pero también deben estar versionadas.

Ejemplo:

```text
ASIR-02-UD03-Q014
ASIR-02-UD03-Q015
ASIR-02-UD03-Q016
```

Pueden compartir la misma competencia y dificultad, pero usar redes, valores o escenarios diferentes.

No se permite que un LLM genere números, topologías, incidencias o casos nuevos en el momento del examen si esos cambios pueden alterar la dificultad o la solución.

## 12. Selección de preguntas

El motor de examen solo podrá seleccionar ítems con:

```text
status = approved
```

La selección debe cumplir el blueprint de la asignatura:

- cobertura de UDs;
- pesos;
- distribución D1-D4;
- tipos de ítem;
- modalidad;
- duración estimada;
- competencias esenciales;
- restricciones de IA.

La selección puede ser aleatoria entre ítems equivalentes previamente aprobados.

## 13. Exámenes ordinarios y recuperación

Un examen ordinario y uno de recuperación deben cubrir las mismas competencias esenciales y mantener dificultad equivalente, pero no reutilizar necesariamente los mismos ítems.

La recuperación utilizará otro conjunto de preguntas aprobadas o variantes equivalentes.

No hay penalización por número de intentos.

El examen solo comienza cuando el alumno lo solicita explícitamente.

## 14. Separación entre contenido visible y solución

La futura aplicación no deberá enviar al cliente la solución, rúbrica privada o claves de corrección antes de entregar la respuesta.

Conceptualmente:

```text
ítem versionado
   ├── contenido visible
   └── contenido privado de corrección
```

La separación física concreta se decidirá al implementar el motor de evaluación.

## 15. Estructura futura de carpetas

Estructura propuesta:

```text
exams/
├── ASIR-00-BLUEPRINT.md
├── ...
├── ASIR-17-BLUEPRINT.md
├── QUESTION_BANK_ARCHITECTURE.md
├── ITEM_TEMPLATE.yml
└── bank/
    ├── ASIR-00/
    │   ├── UD01/
    │   └── ...
    ├── ASIR-01/
    └── ...
```

Al comienzo se podrá usar un archivo YAML por pregunta. Si el volumen hace más conveniente agrupar ítems, la migración deberá conservar IDs y esquema.

## 16. Validación antes de aprobar un ítem

Una pregunta no pasa a `approved` hasta comprobar:

- el enunciado es inequívoco;
- evalúa una competencia real del blueprint;
- no depende de contenido aún no impartido;
- su dificultad D1-D4 está bien clasificada;
- su tiempo estimado es realista;
- la respuesta o rúbrica permite una corrección consistente;
- los datos y comandos son reproducibles;
- no depende innecesariamente de servicios externos inestables;
- contempla seguridad y rollback cuando proceda;
- no contiene secretos reales ni datos personales;
- no exige memorizar sintaxis que en trabajo real se consultaría, salvo que sea una competencia explícita.

## 17. Auditoría del banco

El banco deberá poder responder en cualquier momento a preguntas como:

```text
¿cuántas preguntas aprobadas hay por UD?
¿qué competencias no tienen suficiente cobertura?
¿qué porcentaje es D1/D2/D3/D4?
¿cuántas preguntas prácticas existen?
¿qué ítems llevan demasiado tiempo sin revisarse?
¿qué preguntas dependen de tecnología o normativa susceptible de caducar?
```

Más adelante estas comprobaciones podrán automatizarse con scripts y CI.

## 18. Cantidad mínima antes de comenzar exámenes reales

No se fija todavía un número arbitrario igual para todas las UDs.

La capacidad mínima se calculará desde cada blueprint: debe existir suficiente variedad para construir al menos un examen ordinario y una recuperación equivalentes sin depender de una sola pregunta crítica.

Las UDs con mayor peso o competencias críticas necesitarán más ítems que las UDs de menor peso.

## 19. Papel del tutor IA

El tutor IA puede trabajar con el banco para:

- explicar por qué una respuesta de práctica es incorrecta;
- relacionar el error con la teoría;
- sugerir qué UD repasar;
- explicar una rúbrica después de la entrega;
- resumir patrones de error.

No puede:

- revelar soluciones de un examen activo;
- crear ítems calificables al vuelo;
- alterar la nota decidida por comprobaciones deterministas o rúbricas aprobadas;
- cambiar dificultad o criterios durante un intento.

## 20. Principio final

```text
el banco pregunta
las pruebas verifican
las rúbricas califican
la IA explica
Git conserva la verdad académica
```
