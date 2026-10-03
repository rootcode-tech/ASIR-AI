# ASIR-17 · Proyecto ASIR-AI — Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Módulo:** ASIR-17 · Proyecto ASIR-AI

## 1. Perfil de evaluación

- **Tipo:** evaluación integradora final del ciclo ASIR-AI.
- **Modalidad:** defensa técnica, análisis de arquitectura, demostración controlada, troubleshooting, recuperación y toma de decisiones.
- **Duración orientativa del examen final:** 180-240 minutos, pudiendo dividirse en bloque práctico y defensa oral.
- **Recursos:** documentación propia del proyecto, repositorio, diagramas, ADR, runbooks, terminal, consola de monitorización y documentación oficial indicada por el tribunal.
- **IA:** permitida únicamente en bloques explícitamente marcados como `controlled-AI`; nunca sustituye verificación técnica, razonamiento ni evidencia.
- **Entorno:** infraestructura de laboratorio reproducible, aislada y con datos ficticios.
- **Activación:** el examen solo comienza cuando el alumno lo solicita de forma explícita.

## 2. Cálculo de la calificación

La política general de ASIR-AI se mantiene:

- **60 %:** exámenes de UD ponderados.
- **40 %:** examen final integrador.
- **Mínimo en examen final:** 5.0/10.
- **Mínimo total del módulo:** 5.0/10.

El proyecto, repositorio, documentación, laboratorios y evidencias sirven como contexto y material de verificación, pero **no generan nota por sí mismos**. La nota procede exclusivamente de exámenes.

## 3. Ponderación de los exámenes de UD

| UD | Contenido | Peso |
|---|---|---:|
| UD01 | Problema, requisitos, alcance y criterios de aceptación | 8 % |
| UD02 | Arquitectura, ADR y diseño de red/servicios | 12 % |
| UD03 | Repositorio, Git, documentación e Infrastructure as Code | 10 % |
| UD04 | Plataforma base: red, sistemas, identidad y almacenamiento | 12 % |
| UD05 | Servicios de infraestructura y publicación | 10 % |
| UD06 | Datos, aplicaciones y persistencia | 10 % |
| UD07 | Seguridad, alta disponibilidad y continuidad | 12 % |
| UD08 | Automatización, CI/CD y despliegue reproducible | 10 % |
| UD09 | Observabilidad, backups, pruebas y recuperación | 10 % |
| UD10 | Validación final, memoria, portfolio y defensa | 6 % |

**Total:** 100 %.

## 4. Blueprint del examen final integrador

| Bloque | Competencias principales | Dificultad dominante | Puntos |
|---|---|---|---:|
| A. Requisitos y arquitectura | traducir necesidades a requisitos, restricciones, ADR y arquitectura justificable | D3-D4 | 15 |
| B. Plataforma base | red, Linux/Windows, identidad, almacenamiento, DNS/DHCP y dependencias | D2-D3 | 15 |
| C. Servicios, aplicaciones y datos | publicación, reverse proxy, TLS, aplicaciones, persistencia y operación | D2-D3 | 15 |
| D. Seguridad, HA y continuidad | segmentación, mínimo privilegio, secretos, backups, RPO/RTO, failover y recuperación | D3-D4 | 20 |
| E. Automatización e IaC | Git, CI/CD, Ansible/Terraform, idempotencia y despliegue reproducible | D3-D4 | 15 |
| F. Observabilidad y troubleshooting | métricas, logs, alertas, diagnóstico causal y recuperación | D3-D4 | 10 |
| G. Defensa técnica y trade-offs | explicar decisiones, límites, riesgos, alternativas y evolución | D4 | 10 |

**Total:** 100 puntos.

## 5. Distribución de dificultad

- **D1 · Reconocimiento / comprensión:** 5 %
- **D2 · Aplicación:** 20 %
- **D3 · Diagnóstico / análisis:** 35 %
- **D4 · Integración / decisión:** 40 %

ASIR-17 debe ser el módulo con mayor peso de integración. No se pretende medir memorización de comandos, sino dominio transversal de un sistema complejo.

## 6. Formatos de ítems

El examen podrá combinar:

- análisis de requisitos y restricciones;
- interpretación y corrección de diagramas;
- defensa de ADR;
- revisión de topología de red;
- revisión de reglas de firewall y flujos;
- diagnóstico de DNS, DHCP, routing y TLS;
- diagnóstico de Linux, Windows Server, identidad y permisos;
- despliegue de servicio o aplicación;
- revisión de Docker/Compose/Kubernetes cuando proceda;
- revisión de Terraform/Ansible;
- análisis de pipelines CI/CD;
- SQL y operación de persistencia;
- revisión de logs, métricas, alertas y trazas disponibles;
- prueba de backup y restore;
- recuperación ante fallo inducido;
- explicación oral de decisiones técnicas;
- comparación de alternativas con sus trade-offs;
- bloque `controlled-AI` para evaluar uso crítico y verificable de IA.

## 7. Principio central de evaluación

El proyecto debe demostrar esta cadena:

```text
requisito
  ↓
diseño
  ↓
implementación
  ↓
verificación
  ↓
observabilidad
  ↓
fallo controlado
  ↓
diagnóstico
  ↓
recuperación
  ↓
documentación
```

No se considera dominada una solución que únicamente "funciona" en estado ideal.

## 8. Evidencia técnica exigible

Cuando una respuesta dependa del funcionamiento real del sistema, el alumno debe apoyarla en evidencia verificable, por ejemplo:

- salida de comandos;
- estado de servicios;
- sockets y puertos;
- resolución DNS;
- pruebas de conectividad;
- logs;
- métricas;
- health checks;
- estado de pipelines;
- `terraform plan` / estado gestionado;
- ejecución idempotente de Ansible;
- consultas SQL y estado de la base de datos;
- restauración comprobada;
- pruebas de failover o recuperación;
- historial Git cuando sea relevante.

Una afirmación sin verificación suficiente no equivale a una evidencia.

## 9. Errores críticos

Podrán penalizar gravemente una respuesta o invalidar un bloque cuando exista riesgo real o pérdida de dominio técnico. Ejemplos:

- exponer contraseñas, tokens, claves privadas o secretos en repositorios, logs o capturas;
- ejecutar cambios destructivos sin identificar alcance, backup o rollback;
- usar privilegios excesivos para "hacer que funcione";
- desactivar firewall, TLS, controles de acceso o validaciones sin justificación;
- afirmar que existe backup sin demostrar restauración;
- confundir backup, snapshot, réplica y alta disponibilidad;
- diseñar un SPOF evidente y presentarlo como alta disponibilidad;
- automatizar un procedimiento que no se comprende ni se ha verificado manualmente;
- aplicar IaC sin revisar el plan de cambios;
- modificar varias capas durante un incidente sin aislar variables ni preservar evidencia;
- declarar un incidente resuelto sin pruebas posteriores;
- confiar en una salida de IA como evidencia técnica;
- introducir datos reales sensibles en herramientas o servicios no autorizados;
- falsificar resultados, evidencias, historial o autoría del proyecto.

## 10. Rúbricas específicas

### 10.1 Arquitectura y ADR

- comprensión de requisitos y restricciones: 20 %;
- coherencia de la arquitectura: 25 %;
- dependencias e integración: 20 %;
- seguridad, resiliencia y operación: 20 %;
- justificación de trade-offs: 15 %.

### 10.2 Troubleshooting integral

- recogida inicial de evidencia: 15 %;
- hipótesis razonadas: 20 %;
- aislamiento de causa: 25 %;
- corrección segura y reversible: 20 %;
- validación posterior y documentación: 20 %.

### 10.3 Recuperación ante fallo

- identificación del impacto: 15 %;
- protección de datos y evidencia: 15 %;
- selección del procedimiento de recuperación: 20 %;
- ejecución: 20 %;
- comprobación funcional: 20 %;
- análisis posterior / mejora preventiva: 10 %.

### 10.4 Defensa técnica

- explicación clara de la arquitectura: 20 %;
- dominio de componentes y dependencias: 25 %;
- justificación de decisiones: 20 %;
- capacidad para reconocer límites y alternativas: 15 %;
- respuesta a preguntas y escenarios imprevistos: 20 %.

### 10.5 Uso crítico de IA

Cuando exista bloque `controlled-AI`:

- adecuación de la tarea delegada: 10 %;
- calidad del contexto proporcionado: 10 %;
- detección de errores o afirmaciones no sustentadas: 25 %;
- verificación con herramientas o fuentes autorizadas: 30 %;
- privacidad y seguridad: 15 %;
- conclusión documentada: 10 %.

La calidad de la respuesta del modelo no se califica. Se califica el criterio del alumno.

## 11. Escenarios de fallo inducido

El examen final debe contener al menos un escenario de fallo controlado. Ejemplos adecuados:

- DNS incorrecto;
- certificado vencido o cadena TLS incorrecta;
- servicio caído;
- puerto incorrecto o firewall bloqueando;
- permisos de archivo o servicio defectuosos;
- credencial expirada;
- dependencia de base de datos no disponible;
- volumen o filesystem sin espacio;
- pipeline fallido;
- configuración no idempotente;
- drift de infraestructura;
- alerta de observabilidad que requiere determinar causa real;
- backup que debe restaurarse a un entorno limpio;
- nodo o servicio redundante fuera de servicio.

El objetivo no es sorprender con trucos, sino comprobar un método profesional de diagnóstico.

## 12. Reproducibilidad y automatización

La automatización se evalúa con esta secuencia:

```text
comprender
  ↓
ejecutar manualmente
  ↓
verificar
  ↓
documentar
  ↓
automatizar
  ↓
repetir
  ↓
comprobar idempotencia / estado deseado
  ↓
observar y mantener
```

No se premia convertir en script un procedimiento incorrecto.

## 13. Seguridad de la evaluación

- Todos los dominios, IP, usuarios, certificados, datos y secretos del examen serán ficticios o de laboratorio.
- No se realizará ninguna acción ofensiva contra sistemas externos.
- Las pruebas de seguridad se limitarán al entorno autorizado.
- Las credenciales temporales se invalidarán tras la evaluación cuando proceda.
- No se utilizarán datos personales reales.

## 14. Recuperación del módulo

La recuperación:

- utilizará una arquitectura o escenario distinto pero de dificultad equivalente;
- cubrirá obligatoriamente arquitectura, operación, seguridad, automatización, troubleshooting y recuperación;
- podrá reutilizar competencias, pero no el mismo incidente ni las mismas respuestas;
- mantendrá la exigencia de evidencia verificable;
- sustituirá la nota del módulo conforme al marco general;
- no tendrá penalización ni techo de nota;
- no tendrá límite pedagógico de intentos;
- comenzará únicamente cuando el alumno decida volver a examinarse.

## 15. Criterios de salida del módulo

Antes de considerar ASIR-17 superado, el alumno debe ser capaz de:

1. transformar un problema realista en requisitos técnicos verificables;
2. diseñar una arquitectura coherente y explicar sus dependencias;
3. desplegar y operar red, sistemas, identidad, almacenamiento y servicios;
4. integrar aplicaciones y persistencia de forma segura;
5. aplicar mínimo privilegio, segmentación, secretos y controles de acceso;
6. definir y demostrar una estrategia de backup y recuperación;
7. justificar RPO, RTO y decisiones de continuidad;
8. automatizar infraestructura y despliegues de forma reproducible;
9. mantener cambios bajo control de versiones;
10. detectar y diagnosticar fallos usando evidencia;
11. demostrar observabilidad suficiente para operar el sistema;
12. recuperar el servicio y validar que la recuperación es real;
13. documentar procedimientos, arquitectura, decisiones y riesgos;
14. defender técnicamente el sistema ante preguntas imprevistas;
15. usar IA, cuando proceda, como herramienta auxiliar crítica y verificable, nunca como autoridad.

## 16. Principio final

> El proyecto no se considera terminado porque esté desplegado. Se considera dominado cuando el alumno puede explicar por qué existe, cómo está construido, cómo se verifica, cómo falla y cómo se recupera.
