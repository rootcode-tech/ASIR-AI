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
- `exams/ITEM_TEMPLATE.yml` — plantilla estructurada para un ítem individual.
- `exams/BANK_FORMAT.md` — formato agrupado usado por el banco v0.1.
- `exams/BANK_INDEX.yml` — índice de cobertura y recuento.
- `exams/bank/ASIR-XX.yml` — banco aprobado por asignatura.

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
selección de IDs según blueprint
   ↓
examen ordinario / recuperación
   ↓
validación de cobertura, dificultad y tiempo
```

## Regla sobre IA

La IA puede enseñar, explicar, revisar y ayudar a analizar errores, pero no inventa preguntas calificables durante un examen.

Las preguntas de examen deben existir previamente en el banco, estar versionadas en Git y tener estado `approved`.

## Banco v0.1

El banco mínimo operativo cubre las **18 asignaturas y las 172 UDs**.

Estado actual:

- 18 archivos de banco;
- 172 UDs con cobertura;
- 346 ítems aprobados;
- mínimo de 2 ítems por UD;
- variantes integradoras adicionales donde procede;
- preguntas de uso controlado de IA solo en competencias donde el propio blueprint lo permite.

Este volumen es un suelo operativo, no un techo. Con el uso real del curso se añadirán variantes para reducir repetición y mejorar calibración estadística.

## Estado

- marco común de evaluación: ✅
- plantilla de blueprint: ✅
- blueprints de las 18 asignaturas: ✅
- arquitectura del banco de preguntas: ✅
- formatos de ítem/banco: ✅
- banco mínimo v0.1 de las 18 asignaturas: ✅
- cobertura de las 172 UDs: ✅
- índice de cobertura: ✅
- formularios concretos de examen ordinario/recuperación: ⏳
- validador automático/CI del banco: ⏳
