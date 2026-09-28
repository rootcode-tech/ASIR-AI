# ASIR-12 · Bases de Datos II — Administración de SGBD

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Administrar SGBD de forma profesional: configurar instancias, gestionar seguridad y roles, comprender almacenamiento y concurrencia, optimizar consultas, diseñar recuperación, replicación, alta disponibilidad, auditoría y observabilidad.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Arquitectura interna y ciclo de vida de un SGBD | Especificada |
| UD02 | Instalación, configuración y gestión de instancias | Especificada |
| UD03 | Usuarios, roles, privilegios y separación de funciones | Especificada |
| UD04 | Almacenamiento físico, índices y mantenimiento | Especificada |
| UD05 | Transacciones, bloqueos, concurrencia y aislamiento | Especificada |
| UD06 | Optimización de consultas y análisis de rendimiento | Especificada |
| UD07 | Backup, restore y recuperación punto en el tiempo | Especificada |
| UD08 | Replicación, alta disponibilidad y continuidad | Especificada |
| UD09 | Auditoría, cifrado y hardening del SGBD | Especificada |
| UD10 | Automatización, monitorización y troubleshooting | Especificada |

## Arquitectura pedagógica

```text
arquitectura interna
       ↓
instancia / configuración
       ↓
roles / privilegios
       ↓
storage / índices / mantenimiento
       ↓
transacciones / locks
       ↓
query tuning
       ↓
backup / PITR
       ↓
replicación / HA
       ↓
auditoría / hardening
       ↓
automatización / observabilidad / troubleshooting
```

## Principios

- medir antes de optimizar;
- separar instancia, base y proceso servidor;
- aplicar mínimo privilegio;
- entender MVCC y locks antes de intervenir;
- no crear índices sin justificar;
- distinguir réplica de backup;
- probar PITR;
- auditar accesos;
- proteger secretos;
- versionar scripts/configuración;
- diseñar alertas accionables;
- documentar RCA.

## SGBD de referencia

PostgreSQL será la plataforma principal para administración. Otros motores se utilizarán solo para comparación cuando ayuden a entender conceptos transferibles.

## Relación con módulos posteriores

ASIR-12 conecta directamente con:

- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps/Cloud;
- ASIR-17 Proyecto.

## Evaluación

Los laboratorios, scripts, pruebas de recuperación, tuning y ejercicios son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se crearán datasets de rendimiento, laboratorios de PITR/replicación, incidentes, blueprints de examen y el desarrollo didáctico completo de las 10 UDs.
