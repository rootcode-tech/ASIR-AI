# ASIR-03 · Hardware y CPD — Fundamentos de Hardware

**Estado:** especificación curricular completada  
**UDs:** 9

## Finalidad

Comprender el hardware como infraestructura operativa: seleccionar, mantener, monitorizar y diagnosticar puestos, servidores y elementos básicos de CPD con criterios de rendimiento, disponibilidad, energía y ciclo de vida.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Arquitectura de hardware: CPU, memoria, buses y placas | Especificada |
| UD02 | UEFI/BIOS, POST, arranque y configuración de firmware | Especificada |
| UD03 | Almacenamiento: HDD, SSD, NVMe e interfaces | Especificada |
| UD04 | RAID, redundancia y rendimiento de almacenamiento | Especificada |
| UD05 | Hardware de servidor, gestión remota y componentes empresariales | Especificada |
| UD06 | Energía, fuentes, UPS, protección y continuidad | Especificada |
| UD07 | Racks, cableado, refrigeración y fundamentos de CPD | Especificada |
| UD08 | Dispositivos de red, periféricos y compatibilidad | Especificada |
| UD09 | Diagnóstico, mantenimiento, inventario y ciclo de vida | Especificada |

## Arquitectura pedagógica

```text
CPU / RAM / buses
       ↓
firmware / arranque
       ↓
almacenamiento
       ↓
RAID
       ↓
servidor empresarial
       ↓
energía / UPS
       ↓
rack / CPD / refrigeración
       ↓
interfaces / periféricos
       ↓
diagnóstico + ciclo de vida
```

## Principios

- leer especificaciones con criterio;
- separar capacidad, rendimiento, latencia y disponibilidad;
- RAID no es backup;
- considerar energía, temperatura y mantenibilidad;
- priorizar telemetría y evidencia;
- documentar inventario y ciclo de vida;
- sustituir componentes solo con hipótesis razonada.

## Relación con módulos posteriores

ASIR-03 alimenta directamente:

- ASIR-09 Sistemas II;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps/Cloud en aspectos de infraestructura;
- ASIR-17 Proyecto.

## Evaluación

Los ejercicios y laboratorios son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se crearán bancos de ejercicios, laboratorios completos, blueprints de evaluación y el desarrollo didáctico de cada UD.
