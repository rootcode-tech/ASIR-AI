# ASIR-11 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-11 · Web e Infraestructura — Implantación de Aplicaciones Web

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica de despliegue y operación de aplicaciones web.
- **Modalidad predominante:** despliegue reproducible, publicación segura, mantenimiento y troubleshooting.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** laboratorio reproducible con servidor web, runtime, base de datos, contenedores y reverse proxy cuando proceda.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los laboratorios, simulacros, despliegues de práctica y repeticiones previas no generan nota.

## 2. Cálculo de nota

- Exámenes de UD: **60%**
- Examen final integrador: **40%**
- Mínimo examen final: **5,0**
- Mínimo total: **5,0**
- Recuperación: sustituye la nota de la asignatura.
- Sin penalización por posponer la evaluación.

## 3. Pesos por UD

| UD | Peso dentro del 60% | Justificación |
|---|---:|---|
| UD01 | 8% | Arquitectura web y HTTP sustentan el resto del módulo. |
| UD02 | 10% | Servidor web, virtual hosts y runtime son base operativa. |
| UD03 | 12% | Despliegue con base de datos integra varias capas. |
| UD04 | 8% | CMS añade ciclo de vida, actualización y operación. |
| UD05 | 12% | Contenedores son competencia clave de despliegue moderno. |
| UD06 | 12% | Reverse proxy, TLS y dominios son esenciales para publicación segura. |
| UD07 | 10% | Configuración, secretos y entornos determinan seguridad y reproducibilidad. |
| UD08 | 10% | CI/CD introduce despliegue automatizado y controlado. |
| UD09 | 8% | Seguridad, backups y mantenimiento aseguran operación continuada. |
| UD10 | 10% | Observabilidad, pruebas y troubleshooting integran todo el módulo. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Arquitectura y servidor web | UD01-UD02 | interpretar y configurar stack web | open-lab | D2-D3 | 15 |
| B. App + base de datos | UD03 | desplegar aplicación persistente y validar dependencias | open-lab | D2-D3 | 15 |
| C. CMS / ciclo de vida | UD04 | instalar, actualizar y recuperar | open-lab | D2-D3 | 10 |
| D. Contenedores | UD05 | construir y operar despliegue containerizado | open-lab | D2-D4 | 15 |
| E. Reverse proxy / TLS / secretos | UD06-UD07 | publicar con seguridad y configuración separada | open-lab | D2-D4 | 20 |
| F. CI/CD | UD08 | interpretar, corregir o completar pipeline | open-lab | D2-D4 | 10 |
| G. Operación / observabilidad / incidente | UD09-UD10 | mantener, restaurar y diagnosticar | open-lab | D3-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 5% |
| D2 | Aplicación | 30% |
| D3 | Diagnóstico | 40% |
| D4 | Integración / decisión | 25% |

ASIR-11 evalúa principalmente despliegue, operación y diagnóstico. Memorizar configuraciones no es suficiente.

## 6. Tipos de ítem

Se podrán combinar:

- interpretación de arquitectura web;
- configuración de servidor web;
- virtual hosts;
- runtime de aplicación;
- conexión con base de datos;
- CMS;
- Dockerfile;
- contenedores, redes y volúmenes;
- reverse proxy;
- TLS;
- DNS y dominios a nivel operativo;
- variables de entorno;
- secretos;
- separación dev/test/prod;
- pipelines CI/CD;
- backup/restore;
- health checks;
- logs;
- troubleshooting de despliegue.

## 7. Modalidades

### Open-docs

Se permite documentación oficial para:

- sintaxis de servidores web;
- Docker;
- runtimes;
- TLS;
- CMS;
- CI/CD;
- opciones de configuración.

### Open-lab

Se permite trabajar sobre el entorno real del examen.

El objetivo es demostrar que el alumno puede desplegar y operar, no recordar cada directiva de memoria.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- publicar secretos en repositorio o logs;
- exponer la base de datos directamente sin necesidad;
- usar credenciales por defecto en producción simulada;
- desactivar TLS o validaciones para “hacer que funcione”;
- ejecutar contenedores o servicios con privilegios excesivos sin justificación;
- perder datos persistentes por confundir contenedor con volumen;
- afirmar que existe backup sin probar restore;
- desplegar sin verificar health/readiness;
- realizar cambios irreversibles sin rollback;
- ocultar un fallo de pipeline en lugar de diagnosticarlo.

## 9. Rúbrica de despliegue

| Dimensión | Peso |
|---|---:|
| resultado funcional | 30% |
| arquitectura / configuración | 20% |
| seguridad / secretos | 15% |
| persistencia / datos | 10% |
| verificación | 15% |
| reproducibilidad / documentación | 10% |

## 10. Rúbrica de CI/CD

| Dimensión | Peso |
|---|---:|
| comprensión del flujo | 15% |
| stages/jobs correctos | 20% |
| quality gates | 15% |
| gestión de secretos | 15% |
| despliegue / rollback | 20% |
| diagnóstico de fallo | 15% |

## 11. Rúbrica de troubleshooting web

| Dimensión | Peso |
|---|---:|
| síntoma y alcance | 10% |
| evidencia | 20% |
| identificación de capa | 15% |
| hipótesis | 20% |
| prueba controlada | 15% |
| corrección mínima | 10% |
| validación final / RCA | 10% |

## 12. Exámenes de UD

### UD01

- arquitectura cliente-servidor;
- HTTP;
- frontend/backend;
- servidor web;
- runtime;
- base de datos;
- dependencias.

Modalidad: análisis + open-lab breve.

### UD02

- servidor web;
- virtual hosts;
- puertos;
- runtime;
- logs;
- validación.

Modalidad: open-lab.

### UD03

- desplegar aplicación;
- configurar conexión a BD;
- persistencia;
- migraciones o esquema cuando proceda;
- validación extremo a extremo.

Modalidad: open-lab.

### UD04

- instalar CMS;
- actualizar;
- plugins/extensiones;
- permisos;
- backup;
- recuperación.

Modalidad: open-lab.

### UD05

- Dockerfile;
- imagen;
- contenedor;
- red;
- volumen;
- variables;
- healthcheck.

Modalidad: open-lab.

### UD06

- reverse proxy;
- HTTPS;
- certificados;
- dominios;
- headers básicos;
- publicación.

Modalidad: open-lab.

### UD07

- configuración por entorno;
- secretos;
- .env y límites;
- permisos;
- separación de configuración y código.

Modalidad: open-lab.

### UD08

- pipeline;
- build/test/deploy;
- quality gate;
- secrets;
- fallo de job;
- rollback conceptual/práctico.

Modalidad: open-lab.

### UD09

- hardening;
- mantenimiento;
- backups;
- restore;
- actualización;
- rollback.

Modalidad: open-lab.

### UD10

- logs;
- health checks;
- pruebas;
- observabilidad;
- incidente compuesto;
- RCA.

Modalidad: open-lab integrador.

## 13. Recuperación

La recuperación integral:

- se realiza únicamente cuando el alumno lo solicite;
- usa una aplicación o stack diferente;
- mantiene dificultad equivalente;
- incluye al menos un despliegue completo;
- incluye TLS o reverse proxy;
- incluye persistencia;
- incluye troubleshooting;
- incluye restore o rollback;
- sustituye la nota de ASIR-11;
- no tiene penalización ni límite pedagógico de intentos.

## 14. Requisitos del entorno

El entorno deberá poder recrearse de forma reproducible.

Mínimo:

- una VM Linux;
- servidor web;
- runtime de aplicación;
- base de datos;
- Docker cuando proceda;
- reverse proxy;
- certificados de laboratorio;
- repositorio Git;
- runner o simulación reproducible de CI/CD;
- snapshots o scripts de reset;
- aplicación de ejemplo versionada;
- incidencias inyectables.

No se dependerá de un proveedor cloud concreto para demostrar las competencias esenciales.

## 15. Validación del blueprint

- [x] las 10 UDs están cubiertas;
- [x] servidor web y runtime están representados;
- [x] despliegue con BD tiene peso explícito;
- [x] contenedores tienen evaluación práctica;
- [x] reverse proxy/TLS tienen peso alto;
- [x] secretos se evalúan como requisito de seguridad;
- [x] CI/CD aparece de forma introductoria pero práctica;
- [x] backup exige restore;
- [x] observabilidad y troubleshooting son obligatorios;
- [x] evaluación bajo demanda;
- [x] entorno reproducible.

## 16. Criterio de salida de ASIR-11

ASIR-11 se considera superado cuando el alumno puede, bajo examen:

- explicar una arquitectura web;
- configurar un servidor web y runtime;
- desplegar una aplicación con base de datos;
- operar un CMS;
- containerizar una aplicación;
- publicar mediante reverse proxy y TLS;
- gestionar configuración y secretos;
- interpretar o construir un pipeline básico;
- realizar backup y restore;
- observar y diagnosticar un fallo de despliegue;
- documentar y reproducir el proceso.

El objetivo es pasar de “funciona en mi máquina” a un despliegue reproducible, verificable y mantenible.
