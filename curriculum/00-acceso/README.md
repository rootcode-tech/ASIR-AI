# ASIR-00 · Preparación de acceso a Grado Superior

**Estado:** listo para impartir de forma incremental  
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
