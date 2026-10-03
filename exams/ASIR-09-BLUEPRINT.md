# ASIR-09 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-09 · Sistemas II — Administración de Sistemas Operativos

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica avanzada de administración de sistemas.
- **Modalidad predominante:** open-lab, automatización, diagnóstico y operación de servicios.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab según bloque.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** laboratorio reproducible con Linux y Windows Server, almacenamiento adicional, identidad/directorio, tareas automatizadas y fallos inyectados.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los laboratorios, simulacros, ejercicios y repeticiones previas no generan nota y pueden repetirse sin límite.

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
| UD01 | 10% | Administración avanzada de GNU/Linux es núcleo del módulo. |
| UD02 | 8% | Windows Server y administración remota son esenciales en entorno profesional. |
| UD03 | 10% | Active Directory y GPO son competencias troncales en infraestructuras Windows. |
| UD04 | 10% | Identidad, LDAP y Kerberos conectan autenticación y servicios. |
| UD05 | 10% | LVM, RAID software y cuotas son claves en operación de almacenamiento. |
| UD06 | 12% | Bash y PowerShell convierten procedimientos manuales en operación repetible. |
| UD07 | 8% | Tareas programadas y timers consolidan automatización operativa. |
| UD08 | 8% | Virtualización avanzada y contenedores son puente hacia infraestructura moderna. |
| UD09 | 8% | Backup, restore y recuperación son críticos para continuidad. |
| UD10 | 8% | Logs, monitorización y observabilidad son base del diagnóstico serio. |
| UD11 | 8% | Hardening, mantenimiento y troubleshooting integran todo el módulo. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Linux avanzado | UD01 | administrar servicios, permisos, red y operación avanzada | open-lab | D2-D3 | 15 |
| B. Windows Server / AD | UD02-UD03 | administrar dominio, GPO y acceso remoto | open-lab | D2-D3 | 20 |
| C. Identidad | UD04 | interpretar y operar LDAP/Kerberos a nivel funcional | open-lab | D2-D4 | 10 |
| D. Almacenamiento | UD05 | configurar LVM/RAID software/cuotas y recuperar fallos | open-lab | D2-D3 | 10 |
| E. Automatización | UD06-UD07 | crear scripts/tareas reproducibles e idempotentes cuando proceda | open-lab | D2-D4 | 15 |
| F. Virtualización / contenedores | UD08 | desplegar y verificar aislamiento/recursos | open-lab | D2-D3 | 10 |
| G. Backup / observabilidad / hardening | UD09-UD11 | recuperar, observar y endurecer un sistema | open-lab | D3-D4 | 20 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 5% |
| D2 | Aplicación | 30% |
| D3 | Diagnóstico | 40% |
| D4 | Integración / decisión | 25% |

ASIR-09 prioriza claramente diagnóstico e integración. A este nivel, memorizar comandos aporta poco valor si no se sabe operar y recuperar un sistema.

## 6. Tipos de ítem

Se podrán combinar:

- administración avanzada de Linux;
- systemd;
- permisos, ACL y sudo;
- red y resolución local;
- administración remota;
- Windows Server;
- Active Directory;
- GPO;
- LDAP;
- Kerberos;
- LVM;
- RAID software;
- cuotas;
- Bash;
- PowerShell;
- systemd timers;
- Task Scheduler;
- virtualización;
- contenedores;
- backup/restore;
- logs;
- monitorización;
- hardening;
- troubleshooting integrador;
- RCA técnico breve.

## 7. Modalidades

### Open-docs

Se permite documentación oficial para:

- sintaxis;
- parámetros;
- cmdlets;
- módulos;
- systemd;
- PowerShell;
- LDAP/Kerberos;
- herramientas de backup;
- configuración de almacenamiento.

### Open-lab

Se permite operar directamente sobre máquinas virtuales, directorio, almacenamiento y servicios.

El objetivo es evaluar administración profesional, no memoria literal.

## 8. Principio de automatización

Toda automatización evaluable seguirá esta progresión:

1. comprender el componente;
2. ejecutar manualmente;
3. verificar;
4. diagnosticar fallos;
5. documentar;
6. automatizar;
7. volver a verificar la automatización.

No se considerará dominio copiar un script sin comprender su efecto.

## 9. Errores críticos

Pueden invalidar un ítem práctico:

- borrar datos evitables;
- ejecutar cambios destructivos sin backup o rollback cuando proceda;
- usar permisos excesivos para “hacerlo funcionar”;
- desactivar autenticación o controles de seguridad sin justificación;
- romper un dominio/directorio por cambios no controlados;
- almacenar contraseñas o secretos en texto plano dentro de scripts;
- confundir réplica con backup;
- afirmar recuperación sin probar restore;
- automatizar una operación incorrecta;
- crear una tarea recurrente que cause efectos acumulativos no deseados;
- ignorar logs/evidencia y probar cambios al azar;
- declarar un sistema “seguro” sin validación mínima.

## 10. Rúbrica práctica general

| Dimensión | Peso |
|---|---:|
| resultado correcto | 30% |
| procedimiento / razonamiento | 20% |
| verificación | 20% |
| seguridad / mínimo privilegio / reversibilidad | 15% |
| automatización / repetibilidad | 10% |
| claridad documental | 5% |

## 11. Rúbrica de automatización

| Dimensión | Peso |
|---|---:|
| requisito comprendido | 15% |
| script/configuración funcional | 25% |
| repetibilidad / idempotencia cuando aplique | 20% |
| tratamiento de errores | 15% |
| seguridad / secretos | 10% |
| verificación | 10% |
| documentación | 5% |

## 12. Rúbrica de troubleshooting

| Dimensión | Peso |
|---|---:|
| síntoma y alcance | 10% |
| recogida de evidencia | 20% |
| hipótesis | 20% |
| aislamiento de causa | 20% |
| corrección mínima | 10% |
| validación | 10% |
| RCA / prevención | 10% |

## 13. Exámenes de UD

### UD01

- administración Linux avanzada;
- servicios;
- permisos;
- paquetes;
- red;
- logs;
- acceso remoto.

Modalidad: open-lab.

### UD02

- Windows Server;
- administración remota;
- servicios;
- usuarios;
- PowerShell básico-intermedio.

Modalidad: open-lab.

### UD03

- dominio;
- OU;
- usuarios/grupos;
- GPO;
- herencia;
- validación.

Modalidad: open-lab.

### UD04

- LDAP;
- Kerberos;
- identidad;
- autenticación;
- resolución de incidencias.

Modalidad: open-lab + análisis.

### UD05

- LVM;
- RAID software;
- cuotas;
- expansión;
- fallo controlado;
- recuperación.

Modalidad: open-lab.

### UD06

- Bash;
- PowerShell;
- variables;
- control de flujo;
- funciones;
- manejo de errores;
- automatización.

Modalidad: open-lab.

### UD07

- cron/systemd timers;
- Task Scheduler;
- frecuencia;
- logs;
- reintentos;
- validación.

Modalidad: open-lab.

### UD08

- virtualización;
- recursos;
- redes;
- snapshots;
- contenedores a nivel fundamental;
- aislamiento.

Modalidad: open-lab.

### UD09

- estrategia de backup;
- copia;
- verificación;
- restore;
- recuperación tras fallo.

Modalidad: open-lab.

### UD10

- logs;
- métricas;
- alertas básicas;
- correlación de eventos;
- observabilidad.

Modalidad: open-lab.

### UD11

- hardening;
- mantenimiento;
- parches;
- servicios innecesarios;
- permisos;
- troubleshooting compuesto.

Modalidad: open-lab integrador.

## 14. Recuperación

La recuperación integral:

- se realiza solo cuando el alumno lo solicite;
- usa máquinas o snapshots distintos;
- mantiene dificultad equivalente;
- incluye Linux;
- incluye Windows/AD;
- incluye automatización;
- incluye recuperación o troubleshooting;
- sustituye la nota de ASIR-09;
- no tiene penalización ni límite pedagógico de intentos.

## 15. Requisitos del entorno

El entorno deberá poder recrearse automáticamente o mediante snapshots documentados.

Mínimo:

- 2 VMs GNU/Linux;
- 1 o más Windows Server;
- 1 cliente Windows cuando proceda;
- dominio de laboratorio;
- red interna;
- almacenamiento adicional virtual;
- snapshots base;
- scripts de inyección de fallos;
- repositorio de scripts;
- logs accesibles;
- servicio de backup de laboratorio;
- posibilidad de revertir el entorno.

## 16. Validación del blueprint

- [x] las 11 UDs están cubiertas;
- [x] Linux y Windows Server tienen peso suficiente;
- [x] Active Directory e identidad están representados;
- [x] almacenamiento avanzado se evalúa operativamente;
- [x] Bash y PowerShell tienen evaluación práctica;
- [x] automatización exige comprensión y verificación;
- [x] backups requieren restore;
- [x] observabilidad y hardening tienen peso explícito;
- [x] D3-D4 dominan el examen;
- [x] evaluación bajo demanda;
- [x] entorno reproducible y reversible.

## 17. Criterio de salida de ASIR-09

ASIR-09 se considera superado cuando el alumno puede, bajo examen:

- administrar Linux de forma avanzada;
- administrar Windows Server;
- operar un dominio Active Directory básico;
- comprender identidad con LDAP/Kerberos;
- gestionar almacenamiento avanzado;
- automatizar tareas con Bash y PowerShell;
- programar tareas repetibles;
- operar virtualización/contenedores a nivel básico-intermedio;
- ejecutar y verificar backups/restores;
- interpretar logs y métricas;
- aplicar hardening;
- diagnosticar fallos complejos sin actuar al azar;
- documentar y justificar cada cambio.

El objetivo final es pasar de administrar sistemas manualmente a operarlos de forma repetible, observable, segura y recuperable.
