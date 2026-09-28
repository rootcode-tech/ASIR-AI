# ASIR-13 · Ciberseguridad y Alta Disponibilidad

**Estado:** especificación curricular completada  
**UDs:** 12

## Finalidad

Diseñar, operar y auditar infraestructuras seguras y resilientes integrando gestión de riesgos, hardening, identidad, segmentación, detección, gestión de vulnerabilidades, continuidad, alta disponibilidad y respuesta a incidentes.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Riesgo, amenazas, vulnerabilidades y modelo de defensa | Especificada |
| UD02 | Hardening de sistemas y gestión de configuración segura | Especificada |
| UD03 | Identidad, MFA, PKI, certificados y gestión de secretos | Especificada |
| UD04 | Firewalls, segmentación, ACL y Zero Trust introductorio | Especificada |
| UD05 | IDS/IPS, EDR y fundamentos de SIEM | Especificada |
| UD06 | Gestión de vulnerabilidades y parcheado | Especificada |
| UD07 | Seguridad de servicios web, red y aplicaciones | Especificada |
| UD08 | Copias, recuperación y continuidad de negocio | Especificada |
| UD09 | Alta disponibilidad, clustering y balanceo | Especificada |
| UD10 | Respuesta a incidentes, evidencias y forense básico | Especificada |
| UD11 | Cumplimiento, privacidad, políticas y auditoría | Especificada |
| UD12 | Laboratorio integral de seguridad y resiliencia | Especificada |

## Arquitectura pedagógica

```text
riesgo
  ↓
hardening
  ↓
identidad / MFA / PKI
  ↓
segmentación / firewall
  ↓
detección / SIEM
  ↓
vulnerabilidades / parcheado
  ↓
seguridad de servicios
  ↓
backup / continuidad
  ↓
HA / clustering / balanceo
  ↓
incident response / forense
  ↓
auditoría / cumplimiento
  ↓
laboratorio integral de resiliencia
```

## Principios

- gestionar riesgo, no perseguir seguridad absoluta;
- aplicar mínimo privilegio y mínima conectividad;
- diseñar seguridad desde la arquitectura;
- separar prevención, detección, respuesta y recuperación;
- priorizar vulnerabilidades por contexto, no solo por puntuación;
- no confundir alta disponibilidad con backup;
- preservar evidencias antes de alterar sistemas durante un incidente;
- construir controles medibles y auditables;
- practicar únicamente en entornos autorizados y de laboratorio;
- cerrar incidentes con RCA y acciones preventivas.

## Papel dentro de ASIR-AI

ASIR-13 integra conocimientos de:

- ASIR-02 Redes;
- ASIR-09 Sistemas II;
- ASIR-10 Servicios de Red;
- ASIR-11 Aplicaciones Web;
- ASIR-12 Administración de SGBD.

Y prepara directamente:

- ASIR-16 DevOps/Cloud con seguridad integrada;
- ASIR-17 Proyecto ASIR-AI.

## Evaluación

Los laboratorios, hardening, análisis de riesgos, detecciones, simulaciones de incidentes y auditorías son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se crearán laboratorios defensivos, escenarios de incidentes, datasets de logs, ejercicios de auditoría, blueprints de examen y el desarrollo completo de las 12 UDs.
