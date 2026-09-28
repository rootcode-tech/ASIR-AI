# ASIR-17 · Proyecto ASIR-AI

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Integrar todas las competencias técnicas y profesionales del programa ASIR-AI en un proyecto reproducible, seguro, observable, recuperable, documentado y defendible.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Problema, requisitos, alcance y criterios de aceptación | Especificada |
| UD02 | Arquitectura, ADR y diseño de red/servicios | Especificada |
| UD03 | Repositorio, Git, documentación e Infrastructure as Code | Especificada |
| UD04 | Plataforma base: red, sistemas, identidad y almacenamiento | Especificada |
| UD05 | Servicios de infraestructura y publicación | Especificada |
| UD06 | Datos, aplicaciones y persistencia | Especificada |
| UD07 | Seguridad, alta disponibilidad y continuidad | Especificada |
| UD08 | Automatización, CI/CD y despliegue reproducible | Especificada |
| UD09 | Observabilidad, backups, pruebas y recuperación | Especificada |
| UD10 | Validación final, memoria, portfolio y defensa | Especificada |

## Arquitectura pedagógica

```text
problema / requisitos
        ↓
arquitectura / ADR
        ↓
repositorio / Git / IaC
        ↓
red / sistemas / identidad / storage
        ↓
servicios
        ↓
datos / aplicaciones
        ↓
seguridad / HA / continuidad
        ↓
automatización / CI-CD
        ↓
observabilidad / backup / pruebas / recovery
        ↓
validación / memoria / portfolio / defensa
```

## Principios

- diseñar desde requisitos, no desde herramientas;
- justificar decisiones mediante ADR;
- mantener trazabilidad requisito → implementación → evidencia;
- usar Git como historial técnico del proyecto;
- aplicar IaC solo donde mejore reproducibilidad;
- separar secretos del repositorio;
- integrar seguridad desde el diseño;
- diferenciar disponibilidad, backup y recuperación;
- probar fallos y recuperación;
- observar antes de diagnosticar;
- automatizar solo lo que se comprende manualmente;
- entregar una solución que otro operador pueda mantener.

## Alcance integrador esperado

El proyecto final deberá integrar, cuando corresponda:

- firewall y segmentación;
- VLAN/subredes/routing;
- Linux;
- Windows Server e identidad AD/LDAP;
- DNS/DHCP/NTP;
- almacenamiento;
- base de datos;
- aplicación web;
- reverse proxy y TLS;
- contenedores;
- backups y restore;
- monitorización y logs;
- seguridad y hardening;
- automatización;
- CI/CD;
- cloud e IaC cuando aporten valor;
- documentación operativa;
- continuidad y recuperación ante desastre.

No se obliga a introducir una herramienta únicamente para poder decir que se utilizó. Toda tecnología deberá responder a un requisito o mejorar de forma justificable la operación.

## Evidencia profesional

El repositorio del proyecto deberá poder actuar como pieza principal del portfolio:

- README ejecutivo y técnico;
- arquitectura;
- ADR;
- commits y PR;
- releases;
- IaC;
- pipelines;
- runbooks;
- pruebas;
- incidentes/postmortems;
- recuperación;
- memoria;
- presentación.

## Uso de IA

La IA podrá ayudar en investigación, documentación, revisión, diagnóstico y propuestas, siguiendo siempre:

```text
contexto
  ↓
propuesta
  ↓
contraste con documentación/fuente
  ↓
prueba controlada
  ↓
verificación
  ↓
decisión humana
  ↓
commit / evidencia
```

La IA no sustituye comprensión, validación, seguridad ni responsabilidad técnica.

## Evaluación

Los entregables, repositorio, laboratorios, automatizaciones, memoria y portfolio constituyen evidencia formativa y profesional. La calificación se obtiene mediante exámenes según la política general ASIR-AI.

## Estado de cierre

ASIR-17 queda curricularmente especificado. Con ello quedan especificadas las 18 asignaturas del mapa ASIR-AI. El siguiente paso del proyecto es revisar globalmente el Curriculum Master, diseñar evaluación, laboratorios y ejercicios, y auditar la versión 1.0 antes de iniciar el estudio.
