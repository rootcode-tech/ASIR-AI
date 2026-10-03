# Exams

Sistema de evaluación de ASIR-AI.

## Regla principal

Solo los exámenes generan calificación académica.

No puntúan ejercicios, laboratorios, repositorios, documentación, portfolio ni proyectos. Estos elementos sirven como práctica y evidencia profesional.

Los exámenes solo comienzan cuando el alumno los solicita explícitamente.

## Arquitectura

- `docs/EVALUATION_FRAMEWORK.md` — reglas comunes de evaluación.
- `exams/BLUEPRINT_TEMPLATE.md` — plantilla obligatoria para cada asignatura.
- `exams/ASIR-XX-BLUEPRINT.md` — blueprint específico de cada una de las 18 asignaturas.
- `exams/QUESTION_BANK_ARCHITECTURE.md` — contrato del banco de preguntas versionado.
- `exams/ITEM_TEMPLATE.yml` — plantilla estructurada para cada ítem calificable.
- `exams/bank/` — futuro banco de ítems aprobados, organizado por asignatura y UD.

## Flujo

```text
marco común
   ↓
blueprint por asignatura
   ↓
arquitectura del banco
   ↓
ítems redactados / revisados / aprobados
   ↓
exámenes ordinarios / recuperación
   ↓
validación de cobertura y dificultad
```

## Regla sobre IA

La IA puede enseñar, explicar, revisar y ayudar a analizar errores, pero no inventa preguntas calificables durante un examen.

Las preguntas de examen deben existir previamente en el banco, estar versionadas en Git y tener estado `approved`.

## Estado

- marco común de evaluación: ✅
- plantilla de blueprint: ✅
- blueprints de las 18 asignaturas: ✅
- arquitectura del banco de preguntas: ✅
- plantilla de ítem: ✅
- bancos de preguntas: ⏳
- exámenes finales concretos: ⏳
