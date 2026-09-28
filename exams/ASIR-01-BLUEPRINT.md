# ASIR-01 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-01 · Sistemas I — Implantación de Sistemas Operativos

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica fundamental.
- **Modalidad predominante:** práctica guiada por requisitos + troubleshooting.
- **Duración examen final:** 150 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab según bloque.
- **IA:** no permitida en el examen calificable ordinario.
- **Entorno:** una o más máquinas virtuales Linux/Windows preparadas para examen.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los laboratorios, simulacros y repeticiones previas no generan nota y pueden realizarse tantas veces como sea necesario.

## 2. Cálculo de nota

- Exámenes de UD: **60%**
- Examen final integrador: **40%**
- Mínimo examen final: **5,0**
- Mínimo total: **5,0**
- Recuperación: sustituye la nota de la asignatura.
- Sin penalización por posponer el examen.

## 3. Pesos por UD

| UD | Peso dentro del 60% | Justificación |
|---|---:|---|
| UD01 | 8% | Arquitectura y fundamentos de SO sustentan el resto. |
| UD02 | 8% | Virtualización es el entorno operativo del curso. |
| UD03 | 12% | Instalación, arranque y particionado son competencias base. |
| UD04 | 10% | Sistemas de archivos y montaje son esenciales para operar Linux. |
| UD05 | 12% | Terminal GNU/Linux es competencia troncal. |
| UD06 | 12% | Usuarios, grupos, permisos y ACL son críticos para seguridad y operación. |
| UD07 | 12% | Procesos, servicios, paquetes y logs son núcleo de administración. |
| UD08 | 8% | Windows y PowerShell básico deben quedar operativos. |
| UD09 | 8% | Almacenamiento, backup y recuperación son esenciales. |
| UD10 | 10% | Troubleshooting integra toda la asignatura. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Fundamentos y arquitectura | UD01-UD02 | interpretar hardware/SO/VM y justificar decisiones | closed-book breve | D1-D2 | 10 |
| B. Instalación y filesystem | UD03-UD04 | preparar disco, instalar/montar y validar | open-lab | D2-D3 | 20 |
| C. Linux operativo | UD05-UD07 | administrar por terminal, permisos, procesos y servicios | open-lab | D2-D3 | 30 |
| D. Windows / PowerShell | UD08 | administrar tareas básicas y validar estado | open-lab | D2-D3 | 10 |
| E. Backup y recuperación | UD09 | crear copia, comprobarla y restaurar | open-lab | D2-D3 | 15 |
| F. Incidente integrador | UD10 + anteriores | diagnosticar un sistema con varios fallos | open-lab | D3-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 10% |
| D2 | Aplicación | 40% |
| D3 | Diagnóstico | 35% |
| D4 | Integración / decisión | 15% |

ASIR-01 prioriza aplicación y diagnóstico. Memorizar comandos no es suficiente.

## 6. Tipos de ítem

Se podrán combinar:

- interpretación de arquitectura;
- decisiones de particionado;
- montaje de filesystem;
- comandos de terminal;
- usuarios y grupos;
- permisos y ACL;
- procesos;
- systemd/services;
- gestión de paquetes;
- interpretación de logs;
- tareas PowerShell básicas;
- backup/restore;
- troubleshooting con evidencias;
- respuesta corta justificativa.

## 7. Modalidades

### Closed-book

Solo para fundamentos esenciales:

- conceptos de SO;
- diferencia proceso/servicio;
- filesystem;
- usuario/grupo;
- permiso;
- backup vs restore.

### Open-docs

Se permite documentación oficial para:

- opciones de comandos;
- sintaxis;
- parámetros;
- systemd;
- PowerShell.

### Open-lab

Se permite trabajar sobre la VM, terminal y herramientas locales.

El objetivo es evaluar administración real, no memoria de flags.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- borrar datos cuando no era necesario;
- cambiar permisos a 777 para “hacerlo funcionar” sin justificación;
- ejecutar como root/admin cuando no procede;
- desactivar controles de seguridad;
- afirmar que un servicio funciona sin verificarlo;
- afirmar que un backup es válido sin restaurarlo o comprobarlo;
- modificar múltiples cosas a la vez sin poder identificar cuál resolvió el problema;
- romper deliberadamente la VM fuera del alcance solicitado.

## 9. Rúbrica práctica general

| Dimensión | Peso |
|---|---:|
| resultado correcto | 35% |
| procedimiento | 25% |
| verificación | 20% |
| seguridad / mínimo privilegio / reversibilidad | 15% |
| claridad | 5% |

## 10. Rúbrica de troubleshooting

| Dimensión | Peso |
|---|---:|
| definición correcta del síntoma | 10% |
| recogida de evidencia | 20% |
| hipótesis razonadas | 20% |
| prueba controlada | 20% |
| corrección mínima | 15% |
| validación final | 10% |
| explicación / RCA breve | 5% |

## 11. Exámenes de UD

### UD01

- conceptos de arquitectura;
- CPU/RAM/storage;
- kernel/user space a nivel funcional;
- proceso de arranque;
- razonamiento de recursos.

Modalidad: closed-book breve.

### UD02

- crear/configurar VM;
- CPU/RAM/disco/red;
- snapshots;
- justificar recursos;
- recuperar tras cambio fallido.

Modalidad: open-lab.

### UD03

- instalación;
- boot;
- particionado;
- filesystem;
- validación posterior.

Modalidad: open-lab.

### UD04

- montar/desmontar;
- fstab;
- permisos de montaje;
- diagnosticar mount fallido.

Modalidad: open-lab.

### UD05

- navegación;
- ficheros;
- pipes;
- redirecciones;
- búsqueda;
- ayuda;
- comandos básicos de administración.

Modalidad: open-lab.

### UD06

- usuarios/grupos;
- ownership;
- rwx;
- umask;
- ACL;
- sudo.

Modalidad: open-lab.

### UD07

- procesos;
- señales;
- systemd;
- paquetes;
- logs;
- diagnóstico de servicio.

Modalidad: open-lab.

### UD08

- administración Windows básica;
- servicios;
- usuarios;
- PowerShell;
- validación.

Modalidad: open-lab.

### UD09

- crear backup;
- comprobar integridad;
- restaurar;
- explicar limitaciones.

Modalidad: open-lab.

### UD10

- escenario de fallo compuesto;
- logs;
- permisos;
- servicio;
- filesystem;
- red local si procede;
- RCA.

Modalidad: open-lab.

## 12. Recuperación

La recuperación integral:

- se realiza solo cuando el alumno lo solicite;
- cubre todas las competencias esenciales;
- usa una VM diferente o estado inicial distinto;
- mantiene dificultad equivalente;
- incluye al menos un bloque de troubleshooting;
- sustituye la nota de ASIR-01;
- no tiene penalización ni límite pedagógico de intentos.

## 13. Requisitos del entorno

El entorno de examen deberá poder recrearse de forma reproducible.

Mínimo:

- una VM GNU/Linux;
- una VM Windows o snapshot preparado para UD08;
- snapshots base;
- usuario no privilegiado;
- conectividad local;
- espacio de almacenamiento adicional;
- fallos inyectados mediante script o snapshot;
- logs y servicios controlados.

Los fallos del examen deben poder restaurarse al estado inicial.

## 14. Validación del blueprint

- [x] las 10 UDs están cubiertas;
- [x] Linux tiene peso principal;
- [x] Windows está representado;
- [x] seguridad y mínimo privilegio están incluidos;
- [x] backup exige verificación;
- [x] troubleshooting tiene peso explícito;
- [x] D1 no domina el examen;
- [x] documentación oficial puede usarse donde medir memoria no aporta valor;
- [x] el examen solo se activa bajo demanda;
- [x] el entorno es reproducible y reversible.

## 15. Criterio de salida de ASIR-01

ASIR-01 se considera superado académicamente cuando el alumno puede, bajo examen:

- instalar y arrancar un sistema;
- trabajar por terminal;
- gestionar usuarios y permisos;
- operar procesos y servicios;
- interpretar logs básicos;
- realizar administración Windows elemental;
- crear y restaurar una copia;
- diagnosticar un fallo sencillo de manera estructurada;
- verificar lo que hace.

El objetivo no es memorizar Linux o Windows, sino ser capaz de operar un sistema sin depender de una receta exacta.
