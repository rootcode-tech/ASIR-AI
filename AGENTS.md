# AGENTS.md

## Propósito

Este repositorio contiene el currículo y los materiales de **ASIR-AI** de RootCode Technologies.

## Regla principal

El curso se desarrolla e imparte **por asignaturas cerradas secuencialmente**.

No es necesario esperar a que las 18 asignaturas estén desarrolladas a nivel de lección para comenzar a estudiar. Sí es obligatorio que la asignatura que vaya a impartirse esté preparada antes de comenzar su estudio.

Secuencia pedagógica:

```text
cerrar asignatura N
   ↓
estudiar teoría
   ↓
ejercicios
   ↓
prácticas/laboratorios
   ↓
repaso + simulacro
   ↓
examen solo a petición del alumno
   ↓
corrección y recuperación si hace falta
   ↓
si está aprobada, desarrollar asignatura N+1
```

ASIR-00 es la primera asignatura que se prepara e imparte con este modelo. ASIR-01 no se inicia como siguiente bloque de aprendizaje hasta que ASIR-00 esté aprobado.

Durante el estudio aplicar obligatoriamente `docs/LEARNING_MODEL.md`: enseñar desde cero, no asumir conocimientos no demostrados y permitir tantas explicaciones, repeticiones y preguntas como sean necesarias.

## Fuente de verdad

- Contenido pedagógico: Markdown.
- Metadatos estructurados: `curriculum/curriculum.yml`.
- Historial y revisión: Git.

## Contrato mínimo de una UD

Cada `UDxx.md` debe incluir:

1. Objetivos
2. Conocimientos previos
3. Contenidos
4. Teoría
5. Herramientas
6. Ejercicios
7. Laboratorio
8. Documentación / entregables
9. Competencias transversales
10. Criterios de dominio
11. Preparación del examen
12. Examen

## Reglas editoriales

- No duplicar teoría entre módulos: enlazar al origen cuando sea transversal.
- Introducir una tecnología solo cuando sus prerrequisitos estén cubiertos.
- Priorizar procedimientos reproducibles y verificables.
- Distinguir contenido oficial ASIR de ampliaciones ASIR-AI.
- Mantener nomenclatura estable: `ASIR-XX`, `UDXX`, `LAB-XX`, `EX-XX`.
- Las prácticas no puntúan; los exámenes sí.
- Los exámenes son siempre voluntarios y bajo demanda: solo comienzan cuando el alumno pide explícitamente presentarse.
- No existe penalización pedagógica por retrasar un examen o repetir contenidos.
- Antes de avanzar, priorizar comprensión sobre velocidad o calendario.
- Los ejemplos técnicos deben ser actuales, documentados y reproducibles.
- La experiencia real de una asignatura puede utilizarse para mejorar el diseño de la siguiente sin reducir el nivel final.
