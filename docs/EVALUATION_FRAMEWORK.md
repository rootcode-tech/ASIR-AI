# Marco de Evaluación ASIR-AI

**Versión:** 0.2.0  
**Estado:** arquitectura común vigente  
**Ámbito:** ASIR-00 ... ASIR-17

## 1. Principio general

En ASIR-AI solo una **evaluación calificable explícitamente activada** genera nota.

No puntúan:
- teoría;
- ejercicios;
- laboratorios;
- documentación;
- portfolio;
- proyectos formativos;
- comprobaciones de UD;
- simulacros.

Todo ello sirve para aprender, verificar y decidir si el alumno está preparado.

## 2. Activación

Ningún examen se activa automáticamente.

Solo una petición explícita equivalente a:

> Quiero hacer el examen.

inicia una evaluación calificable.

## 3. Modelo por asignatura

Flujo por defecto:

```text
teoría completa de la asignatura
→ ejercicios guiados
→ ejercicios autónomos
→ prácticas/labs
→ repaso
→ simulacros
→ petición explícita
→ examen final de asignatura
→ recuperación si procede
```

Las comprobaciones de UD son formativas y no generan nota.

Cada blueprint puede establecer gates más estrictos por competencia o dominio, pero no puede convertir prácticas ordinarias en calificación sin una decisión curricular explícita y versionada.

## 4. Qué se mide

- comprensión;
- aplicación;
- diagnóstico;
- justificación;
- verificación;
- seguridad/reversibilidad cuando proceda;
- capacidad de integrar conocimientos.

Memorizar definiciones o comandos sin poder aplicarlos no demuestra dominio.

## 5. Escala

Escala interna: 0,0–10,0.

- <5: no superado;
- ≥5: superado;
- los blueprints pueden exigir mínimos adicionales por bloques críticos.

## 6. Examen final

El examen final debe:
- cubrir los resultados esenciales;
- usar el blueprint de la asignatura;
- tener tiempo realista;
- combinar tipos de ítem adecuados;
- evitar depender de contenido no impartido;
- poder corregirse de forma reproducible.

En módulos extensos puede dividirse en sesiones controladas sin dejar de constituir un único intento académico.

## 7. Recuperación

Si no se supera:
- se analizan errores;
- se vuelve a teoría/práctica;
- el alumno decide cuándo solicitar recuperación;
- se usa una forma equivalente con casos distintos;
- no existe penalización ni techo por recuperar;
- no hay límite pedagógico de intentos.

## 8. Dificultad

- D1: reconocimiento/comprensión;
- D2: aplicación;
- D3: diagnóstico/análisis;
- D4: integración/decisión.

La dificultad depende de la operación cognitiva, no de la longitud de la pregunta.

## 9. Modalidades

- closed_book;
- open_docs;
- open_lab;
- controlled_ai.

El blueprint decide recursos permitidos.

## 10. IA

Por defecto, IA prohibida durante examen calificable.

Puede permitirse cuando la competencia evaluada sea precisamente:
- verificar una respuesta de IA;
- detectar errores;
- contrastar fuentes;
- corregir/validar.

## 11. Ítems y banco

Los ítems calificables:
- se redactan y aprueban previamente;
- no se generan al vuelo durante el examen;
- declaran competencia, dificultad, tiempo y solución/rúbrica;
- permiten ordinario y recuperación equivalentes.

## 12. Prácticas técnicas

Cuando proceda se valora:
- resultado;
- procedimiento;
- verificación;
- seguridad/reversibilidad;
- claridad.

Los pesos exactos pertenecen al blueprint.

## 13. Errores críticos

El blueprint puede invalidar un ítem ante:
- pérdida evitable de datos;
- exposición de secretos;
- permisos deliberadamente inseguros;
- acción irreversible sin salvaguarda;
- confundir backup y réplica;
- afirmar recuperación sin validarla;
- desactivar seguridad sin justificación.

## 14. ASIR-00

ASIR-00 es una adaptación específica al acceso GS:
- usa dominios oficiales;
- modela la convocatoria anual;
- separa la parte general de la preparación específica;
- mantiene simulacros sin nota;
- usa un único examen final bajo demanda;
- exige cobertura suficiente del banco antes de liberar dicho examen.

## 15. Blueprints heredados

Los blueprints v0.1 de asignaturas todavía no activadas pueden conservar decisiones históricas de diseño. Se revisarán cuando cada asignatura pase a ser la asignatura activa.

La fuente operativa es:
1. este marco;
2. el blueprint actualizado de la asignatura activa;
3. AGENTS.md y LEARNING_MODEL.md para el flujo pedagógico.

## 16. Principio final

```text
aprender primero
verificar después
examinar solo cuando el alumno lo pide
calificar con criterios versionados
```
