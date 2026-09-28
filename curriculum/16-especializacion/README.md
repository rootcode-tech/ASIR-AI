# ASIR-16 · Especialización — DevOps, Cloud e IA para Sistemas

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Integrar prácticas modernas de administración de sistemas con Git profesional, contenedores, CI/CD, automatización de configuración, Infrastructure as Code, cloud, Kubernetes, observabilidad, SRE e IA aplicada de forma verificable.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Flujo profesional con Git, ramas, PR, releases y SemVer | Especificada |
| UD02 | Linux para DevOps y automatización reproducible | Especificada |
| UD03 | Docker: imágenes, contenedores, redes y volúmenes | Especificada |
| UD04 | Docker Compose y stacks multi-servicio | Especificada |
| UD05 | CI/CD con pipelines y quality gates | Especificada |
| UD06 | Ansible: inventarios, playbooks, roles e idempotencia | Especificada |
| UD07 | Terraform e Infrastructure as Code | Especificada |
| UD08 | Cloud: IAM, redes, compute, storage y costes | Especificada |
| UD09 | Kubernetes: arquitectura y operación introductoria | Especificada |
| UD10 | Observabilidad, SRE, IA asistida y proyecto DevOps | Especificada |

## Arquitectura pedagógica

```text
Git profesional
      ↓
Linux reproducible
      ↓
Docker
      ↓
Docker Compose
      ↓
CI/CD
      ↓
Ansible
      ↓
Terraform / IaC
      ↓
Cloud
      ↓
Kubernetes
      ↓
Observabilidad / SRE / IA
      ↓
Proyecto DevOps integrador
```

## Principios

- comprender antes de automatizar;
- infraestructura y configuración como código;
- cambios revisables y trazables mediante Git;
- imágenes sin secretos y con versiones explícitas;
- pipelines con quality gates;
- automatización idempotente;
- Terraform state tratado como activo sensible;
- mínimo privilegio en cloud;
- costes como requisito técnico;
- Kubernetes a nivel de fundamentos operativos, no como especialización aislada;
- observabilidad antes de reaccionar;
- SLO y alertas accionables;
- IA como copiloto verificable, nunca como autoridad técnica.

## Regla de automatización

Cada tecnología seguirá la secuencia:

```text
comprender
   ↓
hacer manualmente
   ↓
verificar
   ↓
provocar y diagnosticar fallos
   ↓
documentar
   ↓
automatizar
   ↓
observar y mantener
```

Esto se aplicará especialmente a Ansible, Terraform, CI/CD e IA asistida.

## Papel dentro de ASIR-AI

ASIR-16 es la capa de especialización moderna que conecta todo lo aprendido previamente:

- Linux y Windows;
- redes;
- bases de datos;
- servicios;
- aplicaciones web;
- seguridad;
- documentación;
- Git/GitHub.

Prepara directamente el **ASIR-17 Proyecto ASIR-AI**, donde estas tecnologías se integrarán solo cuando aporten valor arquitectónico real.

## Evaluación

Los repositorios, pipelines, playbooks, IaC, despliegues cloud, manifests, dashboards y proyecto DevOps son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se crearán laboratorios reproducibles, repositorios de práctica, escenarios CI/CD, ejercicios de Ansible/Terraform, labs cloud/Kubernetes, blueprints de examen y el desarrollo completo de las 10 UDs.
