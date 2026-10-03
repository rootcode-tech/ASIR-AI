# ASIR-13 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-13 · Ciberseguridad y Alta Disponibilidad

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica avanzada, transversal y orientada a defensa, resiliencia y continuidad.
- **Modalidad predominante:** análisis de riesgo, configuración defensiva, validación, investigación y respuesta a incidentes.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs/open-lab según bloque; se prioriza consultar documentación real frente a memorizar sintaxis.
- **IA:** no permitida en la evaluación calificable ordinaria, salvo simulaciones formativas o bloques expresamente definidos en el futuro.
- **Entorno:** laboratorio aislado y reproducible, con sistemas vulnerables controlados, logs, capturas, reglas defensivas y snapshots.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

La evaluación se centra en defender, endurecer, detectar, contener, recuperar y justificar decisiones. No busca premiar la ejecución de técnicas ofensivas por sí mismas.

## 2. Cálculo de nota

- Exámenes de UD: **60%**
- Examen final integrador: **40%**
- Mínimo examen final: **5,0**
- Mínimo total: **5,0**
- Recuperación: sustituye la nota de la asignatura.
- Sin penalización por retrasar el examen ni por repetir preparación.

## 3. Pesos por UD

| UD | Peso dentro del 60% | Justificación |
|---|---:|---|
| UD01 | 7% | riesgo, amenazas y vulnerabilidades estructuran el resto del módulo. |
| UD02 | 9% | hardening es una competencia operativa esencial. |
| UD03 | 9% | identidad, MFA, PKI, certificados y secretos son críticos. |
| UD04 | 10% | firewalls, ACL y segmentación son controles troncales. |
| UD05 | 9% | IDS/IPS, EDR y SIEM cubren detección y respuesta. |
| UD06 | 8% | gestión de vulnerabilidades y parcheado requieren priorización. |
| UD07 | 8% | seguridad de servicios web, red y aplicaciones integra capas. |
| UD08 | 8% | backup y continuidad son esenciales para resiliencia. |
| UD09 | 8% | HA, clustering y balanceo requieren diseño y validación. |
| UD10 | 10% | respuesta a incidentes y forense básico integran evidencia y toma de decisiones. |
| UD11 | 6% | cumplimiento, privacidad, políticas y auditoría aportan gobierno. |
| UD12 | 8% | laboratorio integral consolida todas las capacidades. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Riesgo, hardening e identidad | UD01-UD03 | analizar superficie, reducir riesgo y controlar identidad | open-docs | D2-D3 | 20 |
| B. Segmentación y controles de red | UD04 | diseñar y validar firewall/ACL/segmentación | open-lab | D2-D4 | 15 |
| C. Detección y vulnerabilidades | UD05-UD06 | interpretar eventos, priorizar y actuar | open-lab | D3-D4 | 20 |
| D. Seguridad de servicios | UD07 | endurecer y verificar servicios | open-lab | D2-D3 | 10 |
| E. Continuidad y alta disponibilidad | UD08-UD09 | diseñar recuperación y validar resiliencia | open-docs/open-lab | D3-D4 | 15 |
| F. Incidente integral | UD10-UD12 | detectar, contener, preservar evidencia, recuperar y documentar | caso práctico | D3-D4 | 20 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 5% |
| D2 | Aplicación | 25% |
| D3 | Diagnóstico / análisis | 40% |
| D4 | Integración / decisión | 30% |

ASIR-13 exige razonar bajo incertidumbre, priorizar controles y justificar trade-offs.

## 6. Tipos de ítem

Se podrán combinar:

- matrices de riesgo;
- threat modeling básico;
- hardening de Linux/Windows/servicios;
- revisión de permisos y privilegios;
- MFA y gestión de secretos;
- PKI y certificados;
- reglas de firewall y ACL;
- segmentación y microsegmentación introductoria;
- análisis de alertas IDS/IPS/EDR;
- correlación básica de eventos SIEM;
- priorización de vulnerabilidades;
- diseño de parcheado;
- revisión de seguridad HTTP/TLS;
- continuidad, RPO y RTO;
- clustering y balanceo;
- respuesta a incidentes;
- preservación de evidencias;
- timeline básico;
- análisis de logs;
- auditoría técnica;
- caso integral de resiliencia.

## 7. Principio de evaluación

La cadena esperada en seguridad es:

```text
activo
  ↓
amenaza
  ↓
vulnerabilidad
  ↓
riesgo
  ↓
control
  ↓
verificación
  ↓
monitorización
  ↓
respuesta
  ↓
recuperación
```

No se considera válida una defensa que no pueda demostrarse con evidencia.

## 8. Hardening

Se evaluará:

- reducción de superficie de ataque;
- servicios innecesarios;
- configuración segura;
- privilegio mínimo;
- actualización/parcheado;
- permisos;
- autenticación;
- logging;
- protección de secretos;
- verificación posterior.

Rúbrica orientativa:

| Dimensión | Peso |
|---|---:|
| identificación de exposición | 20% |
| propuesta de control | 20% |
| aplicación correcta | 25% |
| verificación | 20% |
| impacto / reversibilidad | 10% |
| documentación | 5% |

## 9. Identidad, MFA, PKI y secretos

Debe distinguirse entre:

- autenticación;
- autorización;
- identidad;
- certificado;
- clave privada;
- secreto;
- sesión;
- privilegio.

Errores especialmente graves:

- exponer una clave privada;
- almacenar secretos en repositorios;
- reutilizar credenciales administrativas;
- conceder privilegios excesivos;
- desactivar validación TLS para resolver un problema;
- aceptar certificados inválidos sin justificar riesgo y compensación.

## 10. Firewall y segmentación

El alumno debe poder justificar:

- origen;
- destino;
- puerto/protocolo;
- dirección del flujo;
- política por defecto;
- excepción mínima necesaria;
- evidencia de que el tráfico permitido funciona;
- evidencia de que el tráfico no permitido queda bloqueado.

No se premiará “abrir todo temporalmente” como solución.

## 11. Detección: IDS/IPS, EDR y SIEM

Se evaluará la capacidad de:

1. interpretar una alerta;
2. diferenciar evento de incidente;
3. correlacionar evidencias;
4. reducir falsos positivos;
5. priorizar severidad;
6. proponer contención;
7. validar impacto.

La simple presencia de una alerta no prueba por sí misma un compromiso.

## 12. Vulnerabilidades y parcheado

Se trabajará con:

- severidad técnica;
- exposición real;
- criticidad del activo;
- explotabilidad;
- impacto;
- controles compensatorios;
- ventana de mantenimiento;
- riesgo de no parchear;
- riesgo de parchear.

La evaluación no premiará priorizar exclusivamente por una cifra CVSS sin contexto.

## 13. Seguridad de servicios

Los casos podrán abarcar:

- SSH;
- HTTP/HTTPS;
- TLS;
- DNS;
- correo;
- SMB/NFS;
- APIs;
- bases de datos;
- servicios internos.

Se debe poder distinguir entre:

- servicio funcional;
- servicio publicado;
- servicio autenticado;
- servicio cifrado;
- servicio endurecido;
- servicio monitorizado.

## 14. Continuidad: backup, RPO y RTO

Debe quedar demostrado que:

```text
backup != réplica
backup != snapshot
HA != backup
replicación != recuperación histórica
```

Se evaluará:

- objetivo de recuperación;
- RPO;
- RTO;
- frecuencia;
- retención;
- aislamiento;
- copia offline/inmutable cuando proceda;
- restore;
- validación de restauración.

## 15. Alta disponibilidad

La evaluación puede incluir:

- balanceo;
- failover;
- quorum a nivel conceptual;
- clustering;
- health checks;
- dependencia compartida;
- SPOF;
- degradación parcial;
- recuperación.

No se considerará HA si existe un único punto de fallo no reconocido.

## 16. Respuesta a incidentes

Flujo esperado:

```text
detección
  ↓
triage
  ↓
contención
  ↓
preservación de evidencia
  ↓
erradicación
  ↓
recuperación
  ↓
validación
  ↓
lecciones aprendidas
```

El alumno debe justificar por qué actúa en ese orden.

## 17. Forense básico y evidencia

La evaluación se limitará a fundamentos defensivos:

- integridad de evidencias;
- timestamps;
- hashing;
- cadena de custodia conceptual;
- logs;
- timeline;
- artefactos básicos;
- documentación de hallazgos.

No se exige análisis forense especializado ni explotación ofensiva avanzada.

## 18. Cumplimiento, privacidad y auditoría

Cuando una pregunta dependa de normativa o requisitos vigentes:

- se proporcionará la norma/fuente necesaria o se permitirá consultarla;
- se evaluará interpretación y aplicación;
- no se exigirá memorizar artículos completos;
- se distinguirá cumplimiento documental de seguridad efectiva.

## 19. Errores críticos

Pueden invalidar un ítem o una parte sustancial del ejercicio:

- borrar evidencias relevantes sin necesidad;
- destruir logs antes de preservarlos;
- desactivar controles de seguridad de forma indiscriminada;
- exponer secretos o claves privadas;
- usar cuentas administrativas para todo;
- abrir `0.0.0.0/0` o equivalente sin justificación;
- afirmar que existe backup sin probar restore;
- afirmar que existe HA sin identificar SPOF;
- confundir replicación con backup;
- comprometer segmentación para “hacer que funcione”;
- parchear o reiniciar sin valorar impacto cuando el caso exige continuidad;
- realizar múltiples cambios simultáneos sin poder atribuir causa/efecto;
- declarar un incidente resuelto sin validación posterior.

## 20. Rúbrica de respuesta a incidente

| Dimensión | Peso |
|---|---:|
| detección y triage | 15% |
| preservación de evidencia | 15% |
| hipótesis y análisis | 20% |
| contención | 15% |
| erradicación / corrección | 10% |
| recuperación | 10% |
| validación | 10% |
| documentación / RCA | 5% |

## 21. Rúbrica de diseño defensivo

| Dimensión | Peso |
|---|---:|
| activos y amenazas | 15% |
| controles propuestos | 20% |
| principio de mínimo privilegio | 15% |
| segmentación | 15% |
| observabilidad | 15% |
| continuidad | 10% |
| justificación / trade-offs | 10% |

## 22. Exámenes de UD

### UD01 · Riesgo, amenazas y vulnerabilidades

- activos;
- amenazas;
- vulnerabilidades;
- impacto;
- probabilidad;
- riesgo;
- controles.

Modalidad: análisis de caso.

### UD02 · Hardening

- baseline;
- servicios;
- permisos;
- actualizaciones;
- logging;
- configuración segura.

Modalidad: open-lab.

### UD03 · Identidad, MFA, PKI y secretos

- autenticación;
- privilegios;
- certificados;
- claves;
- secretos.

Modalidad: caso + configuración.

### UD04 · Firewalls, ACL y Zero Trust introductorio

- políticas;
- reglas;
- segmentación;
- flujos;
- validación.

Modalidad: open-lab.

### UD05 · IDS/IPS, EDR y SIEM

- eventos;
- alertas;
- correlación;
- falsos positivos;
- respuesta.

Modalidad: análisis de logs.

### UD06 · Vulnerabilidades y parcheado

- priorización;
- exposición;
- impacto;
- mantenimiento;
- controles compensatorios.

Modalidad: caso.

### UD07 · Seguridad de servicios web, red y aplicaciones

- TLS;
- exposición;
- autenticación;
- permisos;
- headers y configuración;
- logging.

Modalidad: open-lab.

### UD08 · Copias y continuidad

- backup;
- RPO/RTO;
- retención;
- restore;
- continuidad.

Modalidad: caso + restauración.

### UD09 · Alta disponibilidad

- balanceo;
- clustering;
- failover;
- SPOF;
- health checks.

Modalidad: diseño + validación.

### UD10 · Respuesta a incidentes y forense básico

- triage;
- evidencia;
- contención;
- recuperación;
- timeline.

Modalidad: incidente guiado.

### UD11 · Cumplimiento, privacidad y auditoría

- políticas;
- evidencias;
- cumplimiento;
- privacidad;
- auditoría.

Modalidad: open-docs.

### UD12 · Laboratorio integral

- hardening;
- segmentación;
- detección;
- incidente;
- recuperación;
- documentación.

Modalidad: open-lab integrador.

## 23. Recuperación

La recuperación integral:

- se inicia solo cuando el alumno lo solicite;
- mantiene cobertura y dificultad equivalente;
- usa un escenario distinto;
- incluye segmentación, hardening, análisis de evidencia, continuidad y respuesta a incidentes;
- exige al menos una validación de restore o recuperación;
- sustituye la nota de la asignatura;
- no tiene penalización ni límite pedagógico de intentos.

## 24. Entorno reproducible

Los escenarios deben ser aislados y restaurables mediante snapshots o IaC cuando sea viable.

Podrán emplearse:

- Linux;
- Windows Server;
- firewalls virtuales;
- contenedores;
- servicios web;
- logs sintéticos o reales anonimizados;
- IDS/IPS de laboratorio;
- SIEM de laboratorio;
- capturas de red;
- generadores controlados de eventos;
- backups preparados;
- nodos HA simulados o virtuales.

No se requiere atacar sistemas de terceros ni trabajar fuera de entornos autorizados.

## 25. Validación del blueprint

- [x] las 12 UDs están cubiertas;
- [x] hardening tiene evaluación práctica;
- [x] identidad, PKI y secretos están incluidos;
- [x] firewall y segmentación tienen validación real;
- [x] detección y SIEM se evalúan por evidencia;
- [x] vulnerabilidades se priorizan con contexto;
- [x] backup se diferencia de réplica y HA;
- [x] existe prueba de restore;
- [x] HA exige detectar SPOF;
- [x] respuesta a incidentes preserva evidencia;
- [x] forense básico se mantiene defensivo;
- [x] examen bajo demanda;
- [x] recuperación equivalente.

## 26. Criterio de salida de ASIR-13

ASIR-13 se considera superado cuando el alumno puede, bajo examen:

- evaluar riesgo técnico;
- endurecer sistemas y servicios;
- aplicar mínimo privilegio;
- proteger identidad y secretos;
- diseñar segmentación y firewall;
- interpretar alertas y logs;
- priorizar vulnerabilidades;
- asegurar servicios;
- diseñar backup y continuidad;
- razonar sobre alta disponibilidad;
- responder a un incidente preservando evidencia;
- recuperar y validar el servicio;
- documentar hallazgos y decisiones.

El objetivo final es demostrar que la seguridad no consiste en instalar herramientas, sino en reducir riesgo con controles verificables, detectar desviaciones y recuperar el servicio de forma controlada.
