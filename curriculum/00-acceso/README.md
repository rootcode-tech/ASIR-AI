# ASIR-00 · Preparación de acceso a Grado Superior

**Estado:** listo para impartir de forma incremental · alineado con modelo oficial GS 2025/2026  
**UDs:** 10  
**Finalidad:** preparar el acceso a Grado Superior y construir una base académica directamente útil para ASIR.

## Alineación

La estructura se alinea con las competencias publicadas por la Junta de Andalucía para la preparación del acceso a Grado Superior: Lengua Castellana, Matemáticas, competencia digital, Inglés y competencia de opción. Para un itinerario hacia ASIR se prioriza tecnología e ingeniería cuando corresponda.

> La convocatoria de la prueba puede variar anualmente. Antes de una preparación específica para convocatoria oficial se verificará la normativa vigente y se ajustará el entrenamiento de examen. Véase `docs/OFFICIAL_ALIGNMENT.md`.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Diagnóstico, método de estudio y razonamiento técnico | Lista para impartir |
| UD02 | Aritmética, proporcionalidad, porcentajes y notación científica | Lista para impartir |
| UD03 | Álgebra: expresiones, ecuaciones, sistemas e inecuaciones | Lista para impartir |
| UD04 | Funciones, gráficas y modelización | Lista para impartir |
| UD05 | Geometría, trigonometría y medida | Lista para impartir |
| UD06 | Estadística, probabilidad e interpretación de datos | Lista para impartir |
| UD07 | Fundamentos científico-tecnológicos aplicados | Lista para impartir |
| UD08 | Lengua: comprensión, síntesis y expresión escrita | Lista para impartir |
| UD09 | Inglés funcional y competencia digital | Lista para impartir |
| UD10 | Estrategia de examen y simulacros integrales | Lista para impartir |

## Material de impartición

- `COURSE_READY.md` — guía docente desarrollada de las 10 UDs;
- `OFFICIAL_EXAM_2026_ALIGNMENT.md` — adaptación al formato y competencias del modelo oficial GS 2025/2026;
- `CBCL4_B1_LANGUAGE_ALIGNMENT.md` — desarrollo del bloque de Lengua a partir de los materiales CBCL4_B1 aportados;
- `CBD4_B1_DIGITAL_ALIGNMENT.md` — desarrollo de Competencia Digital a partir de los materiales CBD4_B1 aportados;
- `CBM4_B1_MATH_ALIGNMENT.md` — desarrollo del dominio Números y Cálculo a partir de los materiales CBM4_B1 aportados;
- `EXERCISE_BANK.md` — banco de ejercicios formativos;
- `LABS.md` — prácticas y laboratorios;
- `REVIEW_AND_EXAM_FLOW.md` — repaso, simulacro, examen y recuperación;
- `UD01.md` ... `UD10.md` — especificaciones curriculares fuente;
- `../../exams/ASIR-00-BLUEPRINT.md` — contrato de evaluación;
- `../../exams/bank/ASIR-00.yml` — banco aprobado de ítems calificables.

## Diseño pedagógico

ASIR-00 no se imparte como una colección desconectada de materias. Siempre que sea razonable, los ejercicios se contextualizan en informática, redes, hardware, datos y documentación.

La secuencia es deliberada:

```text
método
  ↓
aritmética
  ↓
álgebra
  ↓
funciones
  ↓
geometría ─┐
estadística├─→ ciencia/tecnología
           │
lengua ────┤
inglés + digital
           ↓
simulacros integrales
```

## Flujo real de estudio

```text
teoría UD01 → UD10
        ↓
ejercicios con ayuda
        ↓
ejercicios autónomos
        ↓
prácticas
        ↓
repaso integral
        ↓
simulacro
        ↓
examen solo a petición expresa
        ↓
corrección + recuperación si procede
        ↓
ASIR-01 cuando ASIR-00 esté aprobado
```

## Evaluación

Solo puntúan los exámenes. Ejercicios, prácticas, laboratorios, diagnósticos y simulacros son formativos.

No existe penalización por repetir teoría, ejercicios, prácticas o simulacros. El examen solo empieza cuando el alumno lo solicita explícitamente.

## Gate de salida

ASIR-00 se considera superado cuando se cumple la política de evaluación definida en su blueprint. Hasta entonces no se abre ASIR-01 como siguiente bloque de estudio.


## Perfil oficial 2025/2026

ASIR-00 ha sido contrastado con los modelos oficiales aportados de Grado Superior y Grado Medio de la Junta de Andalucía.

Para Grado Superior se entrenarán explícitamente:

- los 4 dominios de Lengua Castellana;
- los 3 dominios de Matemáticas;
- los 5 dominios de Competencia Digital;
- Inglés;
- Tecnología e Ingeniería como preparación prioritaria del itinerario ASIR;
- bloques cronometrados de 20 y 40 minutos;
- preguntas de elección entre cuatro respuestas con una correcta;
- expresión escrita de 150-200 palabras;
- comprensión oral con máximo de dos reproducciones en simulación oficial;
- estrategia de test sin penalización por respuesta incorrecta mientras esa regla siga vigente.

El modelo de Grado Medio se utilizará únicamente como escalón didáctico cuando sea útil para introducir una competencia antes de volver al nivel GS.


## Desarrollo de Lengua CBCL4

UD08 ya no se tratará como un único bloque genérico. Los materiales CBCL4_B1 aportados se han integrado como secuencia interna:

```text
comunicación eficaz
→ comunicación no verbal y contexto
→ variedades y registros
→ propiedades textuales
→ tipología textual
→ práctica de expresión/comprensión oral y escrita
```

Las tareas de los materiales fuente sirven también como referencia de diseño: teoría, actividad abierta, test autocorregible, retroalimentación, reintento y entrenamiento temporal.


## Desarrollo de Competencia Digital CBD4

UD09 incorpora ya el Bloque 1 de Competencia Básica Digital N4 a partir de los materiales CBD4_B1 aportados:

```text
búsqueda y verificación
→ IA y prompts
→ organización y propiedad intelectual
→ protección de datos y almacenamiento
→ dispositivos y sincronización
→ ciudadanía digital
→ identidad y huella
→ privacidad
→ colaboración y gestión documental
```

La metodología oficial observada también se conserva: actividades abiertas, ejercicios autocorregibles, tests de 20 preguntas, reintentos formativos y entrenamiento con cuatro opciones y una respuesta correcta.


## Desarrollo de Matemáticas CBM4

UD02 y UD03 incorporan ya el Bloque 1 de Competencia Matemática N4:

```text
números y álgebra
→ proporcionalidad
→ porcentajes
→ matemática financiera
→ problemas combinados
→ comunicación matemática
```

Los cuestionarios de práctica seguirán también la lógica observada en los materiales oficiales: datos variables entre intentos, cuatro opciones, una respuesta correcta, retroalimentación y repetición formativa.
