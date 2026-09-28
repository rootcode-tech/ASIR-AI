# ASIR-01 · Sistemas I — Implantación de Sistemas Operativos

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Construir una base sólida de sistemas operativos antes de entrar en administración avanzada. El alumno debe terminar esta asignatura pudiendo instalar, operar, mantener y diagnosticar sistemas GNU/Linux y Windows en laboratorio.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Arquitectura de computadores y fundamentos de sistemas operativos | Especificada |
| UD02 | Virtualización de laboratorio y gestión de máquinas virtuales | Especificada |
| UD03 | Instalación, arranque, particionado y despliegue de sistemas | Especificada |
| UD04 | Sistemas de archivos, montaje y jerarquía del sistema | Especificada |
| UD05 | Terminal GNU/Linux y administración básica | Especificada |
| UD06 | Usuarios, grupos, permisos, ACL y privilegios | Especificada |
| UD07 | Procesos, servicios, arranque, paquetes y registros | Especificada |
| UD08 | Administración básica de Windows y PowerShell | Especificada |
| UD09 | Almacenamiento, copias de seguridad y recuperación básica | Especificada |
| UD10 | Mantenimiento, diagnóstico y resolución estructurada de incidencias | Especificada |

## Arquitectura pedagógica

```text
hardware + SO
    ↓
virtualización
    ↓
instalación/arranque
    ↓
filesystem
    ↓
Linux shell
    ↓
usuarios/permisos
    ↓
procesos/servicios/logs
    ↓
Windows/PowerShell
    ↓
backup/restore
    ↓
troubleshooting integral
```

## Sistemas de referencia

- GNU/Linux: Debian/Ubuntu Server como base didáctica.
- Windows: Windows cliente y fundamentos administrativos.
- Virtualización: hipervisor de escritorio al inicio; Proxmox aparecerá más adelante.

Las versiones concretas se fijarán al comenzar el curso para no congelar el currículo a una release específica.

## Principios

- comprender antes de automatizar;
- terminal antes que dependencia de GUI;
- logs antes que ensayo aleatorio;
- mínimo privilegio;
- cambios reversibles;
- backup probado;
- documentación reproducible.

## Evaluación

Los ejercicios y laboratorios no puntúan. La evaluación se realiza mediante exámenes de UD y/o examen final según el blueprint que se diseñará en la fase de evaluación.

## Relación con módulos posteriores

ASIR-01 es prerrequisito directo de:

- ASIR-09 Sistemas II;
- ASIR-10 Servicios de Red;
- ASIR-11 Aplicaciones Web;
- ASIR-13 Seguridad y HA;
- ASIR-16 DevOps/Cloud;
- ASIR-17 Proyecto.
