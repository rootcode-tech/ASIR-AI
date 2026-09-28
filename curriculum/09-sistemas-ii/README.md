# ASIR-09 · Sistemas II — Administración de Sistemas Operativos

**Estado:** especificación curricular completada  
**UDs:** 11

## Finalidad

Administrar sistemas GNU/Linux y Windows con un enfoque profesional: identidad, almacenamiento, automatización, virtualización, copias, observabilidad, hardening y troubleshooting avanzado.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Administración avanzada de GNU/Linux | Especificada |
| UD02 | Windows Server y administración remota | Especificada |
| UD03 | Active Directory, dominios y políticas de grupo | Especificada |
| UD04 | Identidad, LDAP, Kerberos y servicios de directorio | Especificada |
| UD05 | LVM, RAID software, cuotas y almacenamiento avanzado | Especificada |
| UD06 | Automatización con Bash y PowerShell | Especificada |
| UD07 | Tareas programadas, systemd timers y operación repetible | Especificada |
| UD08 | Virtualización avanzada y fundamentos de contenedores | Especificada |
| UD09 | Backups, restauración y recuperación ante fallos | Especificada |
| UD10 | Logs, monitorización, auditoría y observabilidad básica | Especificada |
| UD11 | Hardening, mantenimiento y troubleshooting avanzado | Especificada |

## Arquitectura pedagógica

```text
Linux avanzado ───────┐
Windows Server ───────┤
          ↓           │
AD / GPO              │
          ↓           │
LDAP / Kerberos       │
          ↓           │
almacenamiento        │
          ↓           │
Bash / PowerShell     │
          ↓           │
scheduling            │
          ↓           │
virtualización / contenedores
          ↓
backup / recovery
          ↓
logs / observabilidad
          ↓
hardening + troubleshooting
```

## Principios

- operar por CLI y administración remota;
- entender identidad antes de automatizarla;
- separar capas de almacenamiento;
- escribir scripts robustos, no macros frágiles;
- programar tareas con logs y control de errores;
- distinguir VM, contenedor, snapshot, réplica y backup;
- probar restauraciones;
- observar antes de diagnosticar;
- aplicar hardening sin sacrificar operabilidad;
- documentar cambios y causa raíz.

## Papel dentro de ASIR-AI

ASIR-09 es uno de los módulos técnicos centrales del segundo curso. Prepara directamente para:

- ASIR-10 Servicios de Red;
- ASIR-11 Aplicaciones Web;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps, Cloud e IaC;
- ASIR-17 Proyecto.

Docker aparece aquí solo en fundamentos. Su administración y diseño se desarrollarán en ASIR-16 para evitar duplicación.

## Evaluación

Los ejercicios, scripts, laboratorios, incidentes y documentación son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se desarrollarán laboratorios de dominio, scripting, almacenamiento, recuperación, observabilidad, hardening, blueprints de examen y las lecciones completas de las 11 UDs.
