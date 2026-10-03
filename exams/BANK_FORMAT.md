# Formato agrupado del banco de preguntas

**Versión:** 0.1.0  
**Estado:** aprobado

## Objetivo

Para evitar cientos de archivos diminutos, ASIR-AI permite agrupar ítems de una asignatura en un único YAML sin perder IDs estables, trazabilidad ni criterios de corrección.

Cada archivo `exams/bank/ASIR-XX.yml` contiene metadatos comunes y una lista `items`.

## Herencia

Los campos definidos en `defaults` se aplican a todos los ítems salvo que un ítem los sobrescriba.

Campos comunes recomendados:

```yaml
defaults:
  version: 0.1.0
  status: approved
  ai:
    allowed: false
  rubric:
    total_points: 10
    criteria:
      result: 4
      reasoning: 3
      verification: 2
      clarity: 1
```

Cada ítem conserva como mínimo:

- `id`;
- `unit`;
- `title`;
- `competency`;
- `difficulty`;
- `type`;
- `modality`;
- `estimated_time_minutes`;
- `prompt`;
- `expected_answer`;
- `critical_errors` cuando proceda;
- `tags`.

## IDs

Se mantiene el contrato:

```text
ASIR-XX-UDYY-QZZZ
```

Los ítems integradores que combinan varias UDs se asocian a la UD de mayor responsabilidad curricular y añaden `tags: [integrative]`.

## Cobertura mínima v0.1

Cada UD debe disponer, como mínimo, de dos ítems aprobados no equivalentes en texto:

1. uno de aplicación/comprensión;
2. uno de diagnóstico, análisis o integración cuando la naturaleza de la UD lo permita.

Además, cada asignatura debe incluir al menos dos ítems integradores que permitan construir examen ordinario y recuperación con escenarios diferentes.

Esto constituye una **cobertura mínima operativa**, no un límite. Los bancos deberán crecer con variantes adicionales a medida que se use el curso.

## Regla de examen

El motor nunca inventa un ítem. Selecciona IDs aprobados existentes y respeta el blueprint de la asignatura.

## Regla de soluciones

En la futura aplicación, `prompt` podrá viajar al cliente; `expected_answer`, rúbricas privadas y comprobaciones permanecerán en servidor hasta finalizar la entrega.
