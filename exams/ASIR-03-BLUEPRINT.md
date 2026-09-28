# ASIR-03 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-03 · Hardware y CPD — Fundamentos de Hardware

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica fundamental de hardware e infraestructura física.
- **Modalidad predominante:** identificación, dimensionamiento, diagnóstico y toma de decisiones.
- **Duración examen final:** 120-150 minutos orientativos.
- **Recursos permitidos:** open-docs cuando el objetivo sea consultar especificaciones reales; closed-book breve para fundamentos.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** fichas técnicas, inventarios, escenarios de avería y material de laboratorio seguro.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

No se realizará ninguna prueba de riesgo eléctrico ni se exigirá abrir fuentes de alimentación, UPS o equipos con tensión peligrosa.

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
| UD01 | 12% | CPU, RAM, buses y placa son la base conceptual de todo el módulo. |
| UD02 | 8% | UEFI/BIOS y arranque son esenciales para diagnóstico inicial. |
| UD03 | 12% | Almacenamiento físico y sus interfaces son competencia troncal. |
| UD04 | 14% | RAID combina rendimiento, redundancia y diseño de almacenamiento. |
| UD05 | 12% | Hardware de servidor y gestión remota diferencian el entorno profesional. |
| UD06 | 10% | Energía, UPS y continuidad son críticas para operación segura. |
| UD07 | 10% | Rack, cableado, refrigeración y CPD conectan hardware con infraestructura. |
| UD08 | 8% | Compatibilidad e interfaces evitan errores de integración. |
| UD09 | 14% | Diagnóstico, mantenimiento e inventario integran toda la asignatura. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Arquitectura de hardware | UD01-UD02 | interpretar componentes, firmware y arranque | closed-book + análisis | D1-D2 | 15 |
| B. Almacenamiento y RAID | UD03-UD04 | seleccionar, calcular y justificar diseño | open-docs | D2-D3 | 25 |
| C. Hardware de servidor | UD05 | seleccionar componentes y gestión remota | open-docs | D2-D3 | 15 |
| D. Energía y CPD | UD06-UD07 | dimensionar continuidad y condiciones físicas | open-docs | D2-D3 | 20 |
| E. Compatibilidad | UD08 | detectar incompatibilidades e interfaces | open-docs | D2-D3 | 10 |
| F. Incidente de hardware | UD09 + anteriores | diagnosticar avería con evidencia | caso práctico | D3-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 15% |
| D2 | Aplicación | 40% |
| D3 | Diagnóstico | 30% |
| D4 | Integración / decisión | 15% |

ASIR-03 exige saber interpretar especificaciones y diagnosticar, no memorizar catálogos.

## 6. Tipos de ítem

Se podrán combinar:

- identificación de componentes;
- lectura de fichas técnicas;
- compatibilidad CPU/socket/RAM/placa;
- firmware y secuencia de arranque;
- comparación HDD/SSD/NVMe;
- selección de interfaz;
- cálculo de RAID;
- análisis de rendimiento y tolerancia a fallos;
- ECC;
- BMC/IPMI/iDRAC/iLO a nivel funcional;
- dimensionamiento básico de PSU/UPS;
- rack units;
- cableado;
- airflow/refrigeración;
- inventario;
- ciclo de vida;
- diagnóstico por síntomas.

## 7. Modalidades

### Closed-book

Solo para fundamentos esenciales:

- función de CPU/RAM/storage;
- diferencia firmware/SO;
- función básica de RAID;
- diferencia redundancia/backup;
- propósito de UPS;
- concepto de BMC.

### Open-docs

Se permite consultar documentación técnica oficial para:

- sockets;
- compatibilidad;
- consumo;
- capacidades;
- interfaces;
- especificaciones;
- RAID soportado;
- dimensiones;
- requisitos térmicos.

Esto refleja el trabajo real: un técnico profesional consulta especificaciones en lugar de memorizarlas.

## 8. Errores críticos

Pueden invalidar un ítem:

- afirmar que RAID sustituye a un backup;
- recomendar manipulación insegura de tensión de red;
- abrir o reparar internamente PSU/UPS sin entorno autorizado;
- ignorar compatibilidad eléctrica;
- mezclar componentes incompatibles sin detectarlo;
- diseñar redundancia inexistente y afirmar que existe;
- ignorar límites térmicos evidentes;
- diagnosticar sustituyendo piezas al azar sin evidencia;
- destruir información del inventario o del historial de mantenimiento.

## 9. Rúbrica de selección de hardware

| Dimensión | Peso |
|---|---:|
| interpretación de requisitos | 20% |
| compatibilidad | 25% |
| dimensionamiento | 20% |
| justificación técnica | 20% |
| coste/eficiencia/ciclo de vida | 10% |
| claridad documental | 5% |

## 10. Rúbrica de RAID

| Dimensión | Peso |
|---|---:|
| nivel RAID adecuado | 25% |
| capacidad útil | 25% |
| tolerancia a fallos | 20% |
| rendimiento esperado | 15% |
| limitaciones / backup | 15% |

## 11. Rúbrica de troubleshooting

| Dimensión | Peso |
|---|---:|
| síntoma y alcance | 10% |
| evidencia recogida | 20% |
| hipótesis | 20% |
| prueba segura | 20% |
| identificación de causa | 15% |
| corrección / recomendación | 10% |
| documentación | 5% |

## 12. Exámenes de UD

### UD01

- CPU;
- RAM;
- buses;
- chipset/placa;
- arquitectura;
- rendimiento a nivel funcional.

Modalidad: closed-book breve + análisis.

### UD02

- POST;
- UEFI/BIOS;
- boot order;
- firmware;
- diagnóstico de arranque.

Modalidad: caso práctico.

### UD03

- HDD/SSD/NVMe;
- SATA/SAS/PCIe;
- rendimiento;
- resistencia;
- interfaces.

Modalidad: open-docs.

### UD04

- RAID 0/1/5/6/10 a nivel operativo;
- capacidad;
- fallo;
- reconstrucción;
- rendimiento;
- RAID vs backup.

Modalidad: cálculo + caso.

### UD05

- hardware de servidor;
- ECC;
- hot-swap;
- redundancia;
- BMC;
- gestión remota.

Modalidad: open-docs.

### UD06

- PSU;
- consumo;
- UPS;
- autonomía;
- protección;
- continuidad.

Modalidad: cálculo/aplicación.

### UD07

- racks;
- U;
- patch panels;
- cableado;
- airflow;
- refrigeración;
- distribución física.

Modalidad: diseño.

### UD08

- interfaces;
- periféricos;
- compatibilidad;
- adaptación;
- límites.

Modalidad: casos técnicos.

### UD09

- metodología de diagnóstico;
- inventario;
- mantenimiento;
- EOL/EOS;
- ciclo de vida;
- RCA.

Modalidad: caso integrador.

## 13. Recuperación

La recuperación integral:

- se realiza solo cuando el alumno lo solicite;
- usa escenarios de hardware diferentes;
- mantiene dificultad equivalente;
- incluye al menos un ejercicio de RAID;
- incluye compatibilidad;
- incluye un incidente de diagnóstico;
- sustituye la nota de ASIR-03;
- no tiene penalización ni límite pedagógico de intentos.

## 14. Requisitos del entorno

El examen puede utilizar:

- fotos o diagramas de hardware;
- fichas técnicas reales o adaptadas;
- inventarios;
- máquinas apagadas y seguras;
- componentes de baja tensión;
- simulaciones de firmware;
- registros SMART;
- logs de BMC;
- escenarios de fallo documentados.

No se requiere manipular:

- tensión de red;
- fuentes de alimentación abiertas;
- UPS abiertas;
- condensadores;
- baterías peligrosas;
- equipos energizados fuera de prácticas seguras.

## 15. Validación del blueprint

- [x] las 9 UDs están cubiertas;
- [x] RAID tiene peso suficiente;
- [x] servidor/CPD están representados;
- [x] energía y seguridad física están incluidas;
- [x] compatibilidad se evalúa con documentación real;
- [x] diagnóstico tiene peso explícito;
- [x] RAID no se confunde con backup;
- [x] no se exigen prácticas eléctricas peligrosas;
- [x] evaluación bajo demanda;
- [x] recuperación equivalente.

## 16. Criterio de salida de ASIR-03

ASIR-03 se considera superado cuando el alumno puede, bajo examen:

- explicar los componentes principales de un sistema;
- interpretar firmware y arranque;
- seleccionar almacenamiento;
- calcular y justificar RAID;
- comprender hardware de servidor;
- dimensionar energía/UPS a nivel básico;
- diseñar físicamente un pequeño entorno de rack;
- detectar incompatibilidades;
- diagnosticar una avería con evidencia;
- documentar inventario y ciclo de vida;
- trabajar de forma segura.

El objetivo no es memorizar modelos comerciales, sino poder interpretar cualquier plataforma nueva utilizando sus principios y documentación.
