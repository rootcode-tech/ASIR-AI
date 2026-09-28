# Marco de Evaluación ASIR-AI

**Versión:** 0.1.0  
**Estado:** arquitectura común aprobada para diseñar blueprints  
**Ámbito:** ASIR-00 ... ASIR-17

## 1. Principio general

En ASIR-AI **solo los exámenes generan calificación**.

No puntúan:

- ejercicios;
- laboratorios;
- documentación;
- repositorios Git;
- portfolio;
- proyectos;
- presentaciones formativas;
- participación;
- entregables de práctica.

Todos ellos son evidencia de aprendizaje y preparación, pero no modifican la nota.

## 2. Qué se quiere medir

Los exámenes deben comprobar cuatro dimensiones:

1. **Comprensión:** explicar conceptos, relaciones y límites.
2. **Aplicación:** ejecutar o diseñar una solución a partir de requisitos.
3. **Diagnóstico:** interpretar evidencia y localizar una causa.
4. **Justificación:** defender una decisión técnica y sus trade-offs.

No se considera dominio suficiente memorizar comandos, definiciones o recetas sin poder aplicarlos.

## 3. Escala

ASIR-AI utiliza una escala interna de **0,0 a 10,0**.

| Nota | Interpretación |
|---:|---|
| 0,0-4,9 | No alcanza el dominio mínimo |
| 5,0-5,9 | Dominio funcional mínimo |
| 6,0-6,9 | Dominio funcional estable |
| 7,0-8,4 | Dominio autónomo |
| 8,5-9,4 | Dominio avanzado |
| 9,5-10 | Dominio excelente, preciso y justificable |

La escala es propia de ASIR-AI. La equivalencia administrativa con un centro oficial se determinará, si procede, en la fase de alineación final.

## 4. Arquitectura de examen

### Regla de activación

**Ningún examen se activa automáticamente al finalizar una UD o asignatura.**

El alumno decide cuándo quiere presentarse. Antes puede repetir teoría, ejercicios, laboratorios y simulacros tantas veces como necesite, sin penalización.

Solo una solicitud explícita equivalente a **“quiero hacer el examen”** inicia una evaluación calificable.

### 4.1 Examen de UD

Cada UD tendrá un examen breve o medio, disponible bajo demanda.

Objetivo:

- comprobar dominio de la unidad;
- detectar lagunas antes de continuar;
- generar una nota exclusivamente por examen.

Duración orientativa:

- 20-40 min para UDs conceptuales;
- 40-75 min para UDs técnicas;
- hasta 90 min para UDs integradoras.

### 4.2 Examen final de asignatura

Cada asignatura tendrá un examen final integrador, también bajo demanda y únicamente cuando el alumno decida presentarse.

Objetivo:

- comprobar conexiones entre UDs;
- evitar aprobar mediante conocimiento fragmentado;
- evaluar escenarios realistas;
- confirmar autonomía.

Duración orientativa:

- 90-120 min en módulos medios;
- 120-180 min en módulos técnicos/integradores;
- formato adaptado en Inglés, IPE y Proyecto.

## 5. Cálculo de la nota de asignatura

Regla por defecto:

```text
60% media ponderada de exámenes de UD
40% examen final integrador
```

Condiciones:

- el examen final debe obtener **al menos 5,0**;
- la nota total debe ser **al menos 5,0**;
- cuando una asignatura tenga una UD final explícitamente integradora, su examen no sustituye al examen final de asignatura;
- los pesos de las UDs pueden ser diferentes cuando el blueprint justifique que algunas representan mayor carga o criticidad.

## 6. Recuperación

Si no se supera una asignatura, el alumno podrá seguir estudiando y solicitar un **examen de recuperación integral** cuando considere que está preparado.

No hay límite pedagógico de intentos ni penalización por necesitar más tiempo.

Reglas:

- cubre todos los resultados esenciales de la asignatura;
- sustituye la nota de la asignatura por la obtenida en la recuperación;
- no existe penalización ni techo artificial por recuperar;
- debe exigir el mismo nivel de dominio que la convocatoria ordinaria;
- se genera con blueprint equivalente pero preguntas/casos distintos.

## 7. Taxonomía de dificultad

Cada ítem se clasifica como:

### D1 — Reconocimiento y comprensión

- definir;
- identificar;
- interpretar vocabulario;
- reconocer una relación directa.

### D2 — Aplicación

- calcular;
- configurar;
- diseñar;
- transformar;
- utilizar una herramienta con requisitos dados.

### D3 — Diagnóstico y análisis

- interpretar logs;
- encontrar causa;
- comparar hipótesis;
- localizar una configuración incorrecta;
- analizar riesgos o rendimiento.

### D4 — Integración y decisión

- diseñar arquitectura;
- justificar trade-offs;
- priorizar acciones;
- recuperar un sistema;
- integrar varias tecnologías;
- defender una decisión ante restricciones.

## 8. Distribución de dificultad

Plantilla por defecto para exámenes finales técnicos:

| Nivel | Peso orientativo |
|---|---:|
| D1 | 15% |
| D2 | 35% |
| D3 | 30% |
| D4 | 20% |

En UDs iniciales puede aumentar D1/D2. En ASIR-13, ASIR-16 y ASIR-17 se aumentará D3/D4.

## 9. Tipos de ítems permitidos

Se podrán combinar:

- respuesta corta;
- selección múltiple cuando mida discriminación real;
- cálculo;
- interpretación de salida de comandos;
- interpretación de logs;
- completar/configurar fragmentos;
- análisis de arquitectura;
- diseño de red;
- SQL;
- scripting;
- troubleshooting;
- caso técnico;
- comparación razonada;
- defensa oral;
- lectura/escritura técnica en inglés;
- prueba práctica en entorno controlado.

Se evitará que un examen se base principalmente en preguntas de memoria literal.

## 10. Regla de autenticidad

Un buen ítem debe parecerse a una decisión o problema real del ámbito profesional.

Ejemplo débil:

> ¿Qué puerto usa HTTPS?

Ejemplo preferido:

> Un servicio responde por HTTP pero falla por HTTPS. Se muestran certificado, configuración de proxy y logs. Identifica la causa y justifica la corrección.

## 11. Evidencia dentro del examen

En exámenes prácticos se podrá exigir:

- comando utilizado;
- salida relevante;
- configuración;
- consulta;
- diagrama;
- explicación;
- resultado de validación.

No basta con alcanzar accidentalmente el estado final: debe poder explicarse cómo se verificó.

## 12. Puntuación de respuestas prácticas

Rúbrica por defecto:

| Dimensión | Peso |
|---|---:|
| resultado técnicamente correcto | 40% |
| procedimiento / razonamiento | 25% |
| verificación | 20% |
| seguridad / reversibilidad / impacto | 10% |
| claridad | 5% |

Cuando una dimensión no aplique, el blueprint redistribuirá el peso.

## 13. Errores críticos

Un error crítico no implica automáticamente suspender todo el examen, salvo que el blueprint lo defina.

Ejemplos de errores que pueden invalidar un ítem práctico:

- pérdida deliberada o evitable de datos;
- exponer un secreto;
- romper aislamiento o permisos para “hacer que funcione”;
- ejecutar una acción irreversible cuando se pide preservar el sistema;
- confundir backup con réplica en un escenario de recuperación;
- desactivar controles de seguridad sin justificación;
- afirmar una recuperación sin validarla.

## 14. Exámenes con ordenador

Cuando el examen permita ordenador:

- el entorno estará definido;
- se indicará documentación permitida;
- se podrá consultar documentación oficial cuando el objetivo sea operación, no memoria;
- Internet general, IA o repositorios externos solo estarán permitidos si el blueprint lo establece;
- todas las acciones relevantes deben quedar verificables.

## 15. Uso de IA en evaluación

Tres modalidades:

### IA prohibida

Se evalúa dominio autónomo sin asistencia.

### IA permitida con restricciones

Se permite consultar IA, pero el examen evalúa:

- validación;
- detección de errores;
- contraste con documentación;
- corrección;
- explicación.

### IA como objeto del examen

Se proporciona una respuesta generada por IA y se pide auditarla.

Por defecto, los exámenes técnicos de fundamentos se realizarán sin IA; los exámenes de ASIR-07 UD06, ASIR-16 UD10 y partes de ASIR-17 podrán evaluar uso crítico y verificable de IA.

## 16. Open-book vs closed-book

ASIR-AI prioriza capacidad operativa.

Se distinguen:

- **closed-book:** fundamentos que deben dominarse sin apoyo;
- **open-docs:** documentación oficial permitida;
- **open-lab:** terminal, manuales y herramientas permitidos;
- **controlled-AI:** IA explícitamente permitida con obligación de verificación.

El blueprint de cada examen define la modalidad.

## 17. Cobertura

Cada blueprint debe mapear:

`objetivo/criterio de dominio → ítem → dificultad → puntos`

Ninguna UD podrá evaluarse solo con un tipo de pregunta si sus criterios exigen varias habilidades.

## 18. Regla de balance

En módulos técnicos, el examen final no podrá tener más del 35% de puntos basados exclusivamente en recuerdo conceptual.

El resto debe exigir aplicación, diagnóstico o integración.

## 19. Banco de preguntas

Cada UD tendrá un banco suficientemente amplio para permitir:

- convocatoria ordinaria;
- recuperación;
- variantes;
- práctica previa sin revelar el examen real.

Los ítems se etiquetarán con:

- asignatura;
- UD;
- objetivo;
- criterio de dominio;
- dificultad;
- tipo;
- tiempo estimado;
- respuesta esperada;
- rúbrica;
- versión.

## 20. Calidad de un examen

Antes de publicarse, un examen debe superar:

1. cobertura del blueprint;
2. ausencia de ambigüedad;
3. solución verificable;
4. tiempo razonable;
5. dificultad equilibrada;
6. ausencia de dependencia de información no enseñada;
7. ausencia de secretos o datos reales;
8. reproducibilidad de cualquier entorno práctico.

## 21. ASIR-00

ASIR-00 tendrá una adaptación específica:

- simulacros de prueba de acceso;
- matemática, científico-tecnológica, lengua e inglés;
- progresión de tiempo y dificultad;
- examen final integral de acceso.

El detalle deberá alinearse cada año con la convocatoria oficial vigente.

## 22. ASIR-14

Inglés Profesional IT combinará:

- comprensión escrita;
- producción escrita;
- interacción oral;
- documentación técnica;
- entrevista/presentación.

La pronunciación no se evaluará por acento nativo, sino por inteligibilidad profesional.

## 23. ASIR-17

El Proyecto mantiene la regla general: los entregables no puntúan por sí mismos.

El examen final de ASIR-17 puede utilizar el propio proyecto como contexto y evidencia, pero la nota procede de una evaluación explícita que exige:

- explicar decisiones;
- demostrar funcionamiento;
- diagnosticar un fallo;
- defender trade-offs;
- responder preguntas;
- demostrar recuperación.

## 24. Siguiente paso

Crear un **blueprint por asignatura** con:

- cobertura de UDs;
- pesos;
- modalidades;
- duración;
- distribución D1-D4;
- tipos de ítems;
- mínimos;
- recuperación;
- requisitos de entorno.
