# ASIR-12 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-12 · Bases de Datos II — Administración de SGBD

## 1. Perfil de evaluación

- **Tipo de asignatura:** administración avanzada de bases de datos.
- **Modalidad predominante:** open-lab con diagnóstico, rendimiento, recuperación y seguridad.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** documentación oficial del SGBD y apuntes técnicos cuando proceda.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** PostgreSQL como plataforma de referencia, con posibilidad de equivalentes cuando la competencia sea agnóstica al producto.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los laboratorios, simulacros, restauraciones, tuning y troubleshooting previos pueden repetirse sin límite y no generan nota.

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
| UD01 | 8% | Arquitectura y ciclo de vida del SGBD sustentan la administración posterior. |
| UD02 | 10% | Instalación y configuración de instancias son competencias operativas base. |
| UD03 | 10% | Usuarios, roles y privilegios son esenciales para seguridad. |
| UD04 | 10% | Almacenamiento físico, índices y mantenimiento impactan directamente en operación y rendimiento. |
| UD05 | 10% | Transacciones, bloqueos y aislamiento son críticos para integridad y concurrencia. |
| UD06 | 14% | Optimización de consultas y análisis de rendimiento son competencias troncales. |
| UD07 | 14% | Backup, restore y PITR son esenciales para recuperación real. |
| UD08 | 10% | Replicación y alta disponibilidad introducen continuidad del servicio. |
| UD09 | 8% | Auditoría, cifrado y hardening protegen el SGBD. |
| UD10 | 6% | Automatización, monitorización y troubleshooting integran la operación continua. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Instancia y arquitectura | UD01-UD02 | instalar, configurar y justificar parámetros básicos | open-lab | D2-D3 | 15 |
| B. Seguridad y privilegios | UD03 + UD09 | aplicar mínimo privilegio, auditoría y hardening | open-lab | D2-D3 | 15 |
| C. Storage, índices y rendimiento | UD04 + UD06 | medir, diagnosticar y optimizar | open-lab | D2-D4 | 25 |
| D. Concurrencia y transacciones | UD05 | interpretar bloqueos, aislamiento y consistencia | open-lab | D2-D4 | 15 |
| E. Backup / restore / PITR | UD07 | recuperar datos y demostrar RPO/RTO del caso | open-lab | D3-D4 | 20 |
| F. HA / observabilidad / incidente | UD08 + UD10 | diagnosticar replicación, monitorizar y recuperar servicio | open-lab | D3-D4 | 10 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 5% |
| D2 | Aplicación | 30% |
| D3 | Diagnóstico | 40% |
| D4 | Integración / decisión | 25% |

ASIR-12 evalúa principalmente capacidad de operación, diagnóstico y recuperación. Memorizar SQL administrativo no es suficiente.

## 6. Tipos de ítem

Se podrán combinar:

- arquitectura de instancia;
- configuración;
- roles y privilegios;
- separación de funciones;
- tablespaces/storage;
- índices;
- VACUUM/ANALYZE o equivalentes;
- transacciones;
- bloqueos;
- niveles de aislamiento;
- planes de ejecución;
- EXPLAIN/ANALYZE;
- tuning de consultas;
- backup lógico/físico;
- restore;
- PITR;
- replicación;
- failover controlado;
- auditoría;
- cifrado;
- hardening;
- métricas;
- alertas;
- troubleshooting.

## 7. Modalidades

### Closed-book breve

Solo para fundamentos que deben estar interiorizados:

- transacción;
- ACID;
- bloqueo;
- aislamiento;
- índice;
- backup vs réplica;
- RPO/RTO;
- réplica primaria/secundaria a nivel conceptual.

### Open-docs

Se permite documentación oficial para:

- sintaxis administrativa;
- parámetros de configuración;
- catálogo del sistema;
- herramientas de backup/restore;
- replicación;
- observabilidad.

### Open-lab

El alumno deberá operar una instancia real de laboratorio, recoger evidencia y validar los cambios.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- afirmar que una réplica sustituye a un backup;
- dar un backup por válido sin probar restauración;
- borrar o sobrescribir datos sin necesidad;
- ejecutar una recuperación sobre el entorno equivocado;
- conceder privilegios excesivos para “hacerlo funcionar”;
- exponer credenciales o secretos;
- desactivar autenticación o cifrado sin justificación;
- crear índices indiscriminadamente sin medir impacto;
- afirmar mejora de rendimiento sin medición antes/después;
- provocar indisponibilidad evitable por cambios sin rollback;
- afirmar que el failover funciona sin validarlo;
- ignorar consistencia o pérdida de datos en una recuperación.

## 9. Rúbrica de rendimiento

| Dimensión | Peso |
|---|---:|
| definición del problema | 10% |
| medición inicial | 20% |
| interpretación del plan | 25% |
| cambio propuesto | 20% |
| medición posterior | 15% |
| impacto / trade-offs | 10% |

No se acepta “va más rápido” sin evidencia reproducible.

## 10. Rúbrica de backup / restore / PITR

| Dimensión | Peso |
|---|---:|
| estrategia adecuada | 15% |
| ejecución correcta | 20% |
| integridad de la copia | 15% |
| restauración funcional | 25% |
| validación de datos | 15% |
| RPO/RTO y documentación | 10% |

La creación del backup por sí sola no demuestra capacidad de recuperación.

## 11. Rúbrica de troubleshooting

| Dimensión | Peso |
|---|---:|
| síntoma / impacto | 10% |
| métricas / logs / evidencia | 20% |
| hipótesis | 20% |
| prueba controlada | 20% |
| corrección mínima | 15% |
| validación | 10% |
| RCA breve | 5% |

## 12. Exámenes de UD

### UD01

- arquitectura interna;
- procesos;
- memoria;
- catálogo;
- ciclo de vida;
- componentes de instancia.

Modalidad: interpretación + open-lab breve.

### UD02

- instalación;
- inicialización;
- configuración;
- arranque/parada;
- conexiones;
- parámetros.

Modalidad: open-lab.

### UD03

- usuarios;
- roles;
- GRANT/REVOKE;
- separación de funciones;
- mínimo privilegio.

Modalidad: open-lab.

### UD04

- almacenamiento físico;
- índices;
- mantenimiento;
- estadísticas;
- crecimiento.

Modalidad: open-lab.

### UD05

- transacciones;
- bloqueos;
- deadlocks;
- concurrencia;
- niveles de aislamiento.

Modalidad: open-lab con sesiones concurrentes.

### UD06

- EXPLAIN/ANALYZE;
- planes;
- índices;
- estadísticas;
- tuning;
- comparación antes/después.

Modalidad: open-lab.

### UD07

- backup;
- restore;
- WAL o equivalente;
- PITR;
- recuperación validada.

Modalidad: open-lab.

### UD08

- replicación;
- lag;
- sincronía/asynchronía a nivel funcional;
- continuidad;
- failover básico.

Modalidad: open-lab/caso controlado.

### UD09

- auditoría;
- cifrado;
- autenticación;
- hardening;
- secretos.

Modalidad: open-lab.

### UD10

- automatización;
- monitorización;
- métricas;
- alertas;
- troubleshooting;
- RCA.

Modalidad: incidente integrador.

## 13. Recuperación

La recuperación integral:

- se realiza solo cuando el alumno lo solicite;
- utiliza una instancia y dataset diferentes;
- mantiene dificultad equivalente;
- incluye al menos un incidente de rendimiento;
- incluye recuperación de datos;
- incluye seguridad/privilegios;
- incluye troubleshooting;
- sustituye la nota de ASIR-12;
- no tiene penalización ni límite pedagógico de intentos.

## 14. Requisitos del entorno

El entorno debe ser reproducible y restaurable.

Mínimo:

- PostgreSQL de laboratorio;
- dataset conocido y versionado;
- usuarios/roles predefinidos;
- consultas lentas preparadas;
- sesiones concurrentes;
- almacenamiento controlado;
- WAL/archivado o mecanismo equivalente para PITR;
- réplica cuando proceda;
- métricas/logs disponibles;
- snapshots o scripts de reset.

Los exámenes no dependerán de servicios externos inestables.

## 15. Principio de verificación

Toda tarea administrativa relevante deberá cerrar el ciclo:

```text
estado inicial
   ↓
medición / evidencia
   ↓
cambio
   ↓
validación
   ↓
prueba de fallo cuando proceda
   ↓
recuperación
   ↓
validación final
```

En ASIR-12 no basta con que un comando termine sin errores.

## 16. Validación del blueprint

- [x] las 10 UDs están cubiertas;
- [x] rendimiento tiene peso explícito;
- [x] backup exige restore;
- [x] PITR está representado;
- [x] concurrencia se evalúa en laboratorio;
- [x] seguridad y mínimo privilegio están incluidos;
- [x] replicación no se confunde con backup;
- [x] observabilidad y RCA aparecen en el examen;
- [x] D3-D4 predominan;
- [x] examen bajo demanda;
- [x] entorno reproducible.

## 17. Criterio de salida de ASIR-12

ASIR-12 se considera superado cuando el alumno puede, bajo examen:

- desplegar y configurar una instancia;
- administrar roles y privilegios;
- interpretar almacenamiento e índices;
- diagnosticar bloqueos y concurrencia;
- analizar planes de ejecución;
- medir y mejorar rendimiento;
- realizar backup y restore;
- ejecutar una recuperación punto en el tiempo;
- comprender y operar replicación básica;
- aplicar auditoría y hardening;
- monitorizar el SGBD;
- diagnosticar una incidencia con evidencia;
- documentar la recuperación y el RCA.

El objetivo final es poder administrar una base de datos como servicio crítico: con seguridad, medición, recuperación y pruebas, no solo con SQL.
