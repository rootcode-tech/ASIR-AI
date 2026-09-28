# ASIR-02 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-02 · Redes I — Planificación y Administración de Redes

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica fundamental de redes.
- **Modalidad predominante:** cálculo, diseño, configuración, captura y troubleshooting.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab según bloque.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** simulador/emulador o laboratorio reproducible con hosts, switches y routers virtuales cuando proceda.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los ejercicios, laboratorios y simulacros previos pueden repetirse sin límite y no generan nota.

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
| UD01 | 8% | Modelos, encapsulación y herramientas sustentan todo diagnóstico posterior. |
| UD02 | 7% | Ethernet y capa 2 son base de switching y captura. |
| UD03 | 15% | IPv4, subnetting y VLSM son competencias nucleares. |
| UD04 | 10% | IPv6 debe manejarse de forma operativa, no solo conceptual. |
| UD05 | 10% | Switching y STP son esenciales en redes LAN. |
| UD06 | 12% | VLAN y trunking son base de segmentación. |
| UD07 | 12% | Routing estático y fundamentos dinámicos son troncales. |
| UD08 | 10% | DHCP, DNS y NAT/PAT conectan red con servicios. |
| UD09 | 6% | Wi-Fi y movilidad deben comprenderse con foco operativo y de seguridad. |
| UD10 | 10% | Captura, documentación y troubleshooting integran toda la asignatura. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Fundamentos y Ethernet | UD01-UD02 | interpretar capas, tramas, MAC y encapsulación | closed-book breve | D1-D2 | 10 |
| B. IPv4 / VLSM | UD03 | calcular, planificar y justificar direccionamiento | open-docs limitada | D2-D3 | 20 |
| C. IPv6 | UD04 | direccionar, interpretar prefijos y diagnosticar conectividad | open-lab | D2-D3 | 10 |
| D. Switching / VLAN / STP | UD05-UD06 | segmentar, configurar y verificar LAN | open-lab | D2-D3 | 20 |
| E. Routing | UD07 | configurar rutas y validar tablas/alcance | open-lab | D2-D4 | 15 |
| F. Servicios de apoyo | UD08-UD09 | DHCP/DNS/NAT/Wi-Fi y seguridad básica | open-lab | D2-D3 | 10 |
| G. Incidente de red | UD10 + anteriores | captura, hipótesis, aislamiento y RCA | open-lab | D3-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 10% |
| D2 | Aplicación | 35% |
| D3 | Diagnóstico | 35% |
| D4 | Integración / decisión | 20% |

ASIR-02 prioriza aplicación y diagnóstico con una presencia significativa de integración.

## 6. Tipos de ítem

Se podrán combinar:

- subnetting;
- VLSM;
- IPv6;
- interpretación de tablas de routing;
- análisis de tramas;
- diseño de topologías;
- configuración de VLAN/trunks;
- STP;
- rutas estáticas;
- DHCP;
- DNS básico;
- NAT/PAT;
- Wi-Fi;
- packet capture;
- interpretación de ping/traceroute/arp/ip/route;
- troubleshooting por capas;
- documentación de red.

## 7. Modalidades

### Closed-book

Solo para fundamentos esenciales:

- OSI/TCP-IP;
- encapsulación;
- diferencia MAC/IP;
- conceptos de switching/routing;
- función de gateway;
- concepto de subnetting.

### Open-docs

Se permite documentación oficial para:

- sintaxis de comandos;
- tablas de prefijos;
- opciones específicas;
- configuración de dispositivos.

### Open-lab

Se permite trabajar sobre el laboratorio, capturar tráfico y consultar salidas de dispositivos.

El objetivo es evaluar razonamiento de red, no memoria de comandos propietarios.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- asignar direccionamiento solapado sin detectarlo;
- configurar gateway fuera de la subred;
- romper segmentación mezclando VLAN sin justificación;
- crear bucles de capa 2 evitables;
- desactivar STP para “resolver” un problema;
- exponer servicios por NAT/PAT sin necesidad ni control;
- afirmar que hay conectividad sin verificarla;
- interpretar una captura ignorando la evidencia;
- cambiar varias capas simultáneamente sin aislar la causa;
- ocultar un fallo documental en vez de corregirlo.

## 9. Rúbrica de subnetting / VLSM

| Dimensión | Peso |
|---|---:|
| identificación de necesidades | 15% |
| cálculo correcto | 35% |
| ausencia de solapamientos | 20% |
| uso eficiente del espacio | 15% |
| documentación / justificación | 15% |

## 10. Rúbrica de troubleshooting de red

| Dimensión | Peso |
|---|---:|
| definición del síntoma | 10% |
| elección de capa / alcance | 15% |
| evidencia recogida | 20% |
| hipótesis | 20% |
| prueba controlada | 15% |
| corrección mínima | 10% |
| validación / RCA | 10% |

## 11. Exámenes de UD

### UD01

- OSI/TCP-IP;
- encapsulación;
- puertos/protocolos a nivel funcional;
- herramientas básicas de diagnóstico.

Modalidad: closed-book breve + interpretación.

### UD02

- MAC;
- Ethernet;
- switching básico;
- medios;
- topologías;
- análisis de trama.

Modalidad: open-docs/open-lab.

### UD03

- IPv4;
- máscara/prefijo;
- network/broadcast;
- hosts;
- subnetting;
- VLSM;
- planificación.

Modalidad: cálculo + diseño.

### UD04

- IPv6;
- tipos de dirección;
- prefijos;
- autoconfiguración;
- coexistencia;
- diagnóstico.

Modalidad: open-lab.

### UD05

- switching;
- MAC table;
- STP;
- puertos;
- convergencia básica.

Modalidad: open-lab.

### UD06

- VLAN;
- access/trunk;
- etiquetado;
- segmentación;
- validación.

Modalidad: open-lab.

### UD07

- routing;
- tablas;
- rutas estáticas;
- default route;
- fundamentos de routing dinámico;
- diagnóstico.

Modalidad: open-lab.

### UD08

- DHCP;
- DNS;
- NAT/PAT;
- dependencias;
- pruebas.

Modalidad: open-lab.

### UD09

- Wi-Fi;
- canales;
- cobertura;
- autenticación/cifrado;
- movilidad;
- diagnóstico básico.

Modalidad: caso aplicado.

### UD10

- captura;
- documentación;
- troubleshooting;
- diseño integral;
- RCA.

Modalidad: open-lab integrador.

## 12. Recuperación

La recuperación integral:

- se activa solo cuando el alumno lo solicite;
- cubre cálculo, configuración y troubleshooting;
- utiliza topología distinta;
- mantiene dificultad equivalente;
- incluye al menos un ejercicio de subnetting/VLSM;
- incluye al menos un incidente de red;
- sustituye la nota de ASIR-02;
- no tiene penalización ni límite pedagógico de intentos.

## 13. Requisitos del entorno

El entorno deberá ser reproducible y restaurable.

Mínimo:

- 2 o más hosts;
- 2 switches virtuales o equivalentes;
- 1 o más routers;
- varias VLAN;
- IPv4 e IPv6;
- DHCP/DNS de laboratorio;
- NAT/PAT cuando proceda;
- herramienta de captura;
- snapshots o configuración base;
- incidencias inyectables.

Herramientas posibles:

- Packet Tracer;
- GNS3;
- EVE-NG;
- Linux network namespaces;
- tcpdump/Wireshark;
- routers/switches virtuales equivalentes.

La herramienta concreta podrá variar; la competencia evaluada no dependerá de una marca.

## 14. Validación del blueprint

- [x] las 10 UDs están cubiertas;
- [x] subnetting/VLSM tiene peso alto;
- [x] IPv6 se evalúa operativamente;
- [x] switching/VLAN/routing tienen peso práctico;
- [x] DHCP/DNS/NAT están integrados;
- [x] Wi-Fi está representado;
- [x] packet capture y troubleshooting tienen peso explícito;
- [x] D1 no domina el examen;
- [x] comandos propietarios no son el objetivo;
- [x] examen bajo demanda;
- [x] entorno reproducible.

## 15. Criterio de salida de ASIR-02

ASIR-02 se considera superado cuando el alumno puede, bajo examen:

- explicar cómo viaja un paquete/trama;
- planificar IPv4 con subnetting/VLSM;
- trabajar con IPv6 básico;
- configurar switching y VLAN;
- interpretar STP;
- configurar routing básico;
- comprender DHCP/DNS/NAT;
- diagnosticar conectividad por capas;
- capturar tráfico y extraer evidencia;
- documentar una red;
- verificar cada cambio.

El objetivo final es dejar de “probar cosas” y aprender a razonar la red capa por capa.
