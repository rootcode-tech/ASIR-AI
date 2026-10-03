# ASIR-04 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-04 · Bases de Datos I — Gestión de Bases de Datos

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica fundamental de bases de datos relacionales.
- **Modalidad predominante:** modelado, SQL, integridad y resolución de casos.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab en bloques operativos; closed-book breve para fundamentos esenciales.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** PostgreSQL como SGBD de referencia, con datasets y esquemas reproducibles.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los ejercicios, laboratorios, consultas de práctica y simulacros previos pueden repetirse sin límite y no generan nota.

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
| UD01 | 6% | Los modelos de datos y sistemas de información dan contexto al resto. |
| UD02 | 12% | El modelo entidad-relación es la base del diseño conceptual. |
| UD03 | 12% | El modelo relacional, claves y restricciones son núcleo del diseño lógico. |
| UD04 | 12% | La normalización evita anomalías y mejora la calidad del esquema. |
| UD05 | 10% | DDL y restricciones convierten el diseño en una estructura real. |
| UD06 | 8% | DML debe ejecutarse con control y seguridad. |
| UD07 | 12% | SELECT, agregación y funciones son competencias operativas esenciales. |
| UD08 | 14% | JOIN, subconsultas y vistas concentran gran parte del razonamiento SQL. |
| UD09 | 8% | Transacciones e integridad introducen comportamiento multioperación. |
| UD10 | 6% | Usuarios, privilegios y backup/restore son la base operativa previa a ASIR-12. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Modelado conceptual | UD01-UD02 | interpretar requisitos y construir ER | closed-book + caso | D1-D3 | 15 |
| B. Modelo relacional / normalización | UD03-UD04 | transformar, justificar claves y normalizar | open-docs limitada | D2-D4 | 20 |
| C. DDL / DML / integridad | UD05-UD06 | crear y modificar esquema/datos con seguridad | open-lab | D2-D3 | 15 |
| D. Consultas SQL | UD07-UD08 | resolver consultas simples y avanzadas | open-lab | D2-D4 | 30 |
| E. Transacciones | UD09 | razonar atomicidad, concurrencia e integridad | open-lab + análisis | D2-D3 | 10 |
| F. Operación básica | UD10 | usuarios, privilegios y restore básico | open-lab | D2-D3 | 10 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 10% |
| D2 | Aplicación | 40% |
| D3 | Diagnóstico / análisis | 30% |
| D4 | Integración / diseño | 20% |

ASIR-04 prioriza diseñar y consultar correctamente; memorizar sintaxis sin comprender el modelo no es suficiente.

## 6. Tipos de ítem

Se podrán combinar:

- interpretación de requisitos;
- diagrama entidad-relación;
- cardinalidad y participación;
- transformación ER → relacional;
- identificación de claves;
- normalización 1FN/2FN/3FN;
- detección de anomalías;
- CREATE/ALTER/DROP controlado;
- restricciones PK/FK/UNIQUE/CHECK/NOT NULL;
- INSERT/UPDATE/DELETE seguros;
- SELECT;
- filtros;
- agregaciones;
- GROUP BY/HAVING;
- JOIN;
- subconsultas;
- vistas;
- transacciones;
- rollback;
- permisos;
- backup/restore básico;
- troubleshooting de consultas y restricciones.

## 7. Modalidades

### Closed-book

Solo para fundamentos esenciales:

- entidad;
- atributo;
- relación;
- clave primaria/foránea;
- integridad referencial;
- normalización a nivel conceptual;
- transacción;
- diferencia entre esquema y datos.

### Open-docs

Se permite documentación oficial de PostgreSQL para:

- sintaxis concreta;
- funciones;
- tipos;
- opciones de DDL;
- comandos administrativos básicos.

### Open-lab

Se permite trabajar contra una instancia PostgreSQL de examen.

El objetivo es evaluar capacidad real de diseño y consulta, no memoria de cada palabra reservada.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- ejecutar UPDATE o DELETE masivo sin filtro cuando el caso exige preservar datos;
- eliminar una tabla o esquema sin necesidad;
- desactivar restricciones para “hacer que funcione” sin justificación;
- duplicar datos de forma intencionada ignorando el modelo;
- afirmar que una consulta es correcta sin comprobar su resultado;
- usar privilegios excesivos cuando se pide mínimo privilegio;
- afirmar que existe backup sin comprobar restauración o contenido;
- modificar datos de producción simulada cuando bastaba con una transacción de prueba;
- ocultar una anomalía de modelado en vez de corregirla.

## 9. Rúbrica de modelado

| Dimensión | Peso |
|---|---:|
| interpretación de requisitos | 20% |
| entidades/atributos | 20% |
| relaciones/cardinalidades | 25% |
| claves/restricciones | 20% |
| claridad/justificación | 15% |

## 10. Rúbrica de normalización

| Dimensión | Peso |
|---|---:|
| detección de dependencia/anomalía | 20% |
| aplicación correcta de forma normal | 30% |
| descomposición válida | 25% |
| preservación de información | 15% |
| justificación | 10% |

## 11. Rúbrica de SQL

| Dimensión | Peso |
|---|---:|
| resultado correcto | 35% |
| consulta lógicamente correcta | 30% |
| uso adecuado de JOIN/filtros/agregación | 15% |
| verificación | 10% |
| legibilidad / seguridad | 10% |

## 12. Exámenes de UD

### UD01

- sistemas de información;
- dato vs información;
- modelos;
- necesidad de persistencia;
- requisitos de datos.

Modalidad: closed-book breve + caso.

### UD02

- entidad-relación;
- atributos;
- identificadores;
- relaciones;
- cardinalidad;
- diseño conceptual.

Modalidad: caso de modelado.

### UD03

- tablas;
- filas/columnas;
- PK/FK;
- restricciones;
- transformación desde ER.

Modalidad: diseño relacional.

### UD04

- dependencias;
- anomalías;
- 1FN;
- 2FN;
- 3FN;
- justificación de diseño.

Modalidad: caso de normalización.

### UD05

- CREATE TABLE;
- tipos;
- PK/FK;
- CHECK;
- UNIQUE;
- ALTER;
- esquema.

Modalidad: open-lab.

### UD06

- INSERT;
- UPDATE;
- DELETE;
- WHERE;
- integridad;
- transacción protectora cuando proceda.

Modalidad: open-lab.

### UD07

- SELECT;
- WHERE;
- ORDER BY;
- funciones;
- agregaciones;
- GROUP BY;
- HAVING.

Modalidad: open-lab.

### UD08

- INNER/LEFT JOIN;
- múltiples tablas;
- subconsultas;
- vistas;
- consultas avanzadas.

Modalidad: open-lab.

### UD09

- ACID;
- BEGIN/COMMIT/ROLLBACK;
- integridad;
- concurrencia conceptual;
- bloqueo/aislamiento introductorio.

Modalidad: open-lab + análisis.

### UD10

- usuarios;
- roles;
- GRANT/REVOKE;
- mínimo privilegio;
- backup/restore básico;
- operación elemental.

Modalidad: open-lab.

## 13. Recuperación

La recuperación integral:

- se activa únicamente cuando el alumno lo solicite;
- utiliza un dominio de datos distinto;
- mantiene dificultad equivalente;
- incluye modelado;
- incluye normalización;
- incluye SQL práctico;
- incluye al menos una consulta con JOIN;
- incluye una operación de integridad/transacción;
- sustituye la nota de ASIR-04;
- no tiene penalización ni límite pedagógico de intentos.

## 14. Requisitos del entorno

El entorno deberá poder reconstruirse automáticamente.

Mínimo:

- PostgreSQL;
- base de datos de examen aislada;
- usuario limitado;
- dataset reproducible;
- scripts de creación/reset;
- expected results para consultas;
- fixtures para restricciones;
- backup de laboratorio;
- acceso a documentación oficial cuando el blueprint lo permita.

Los datasets no deben contener información personal real.

## 15. Corrección automatizable

Cuando sea posible, las respuestas SQL podrán verificarse mediante tests:

- conjunto de filas esperado;
- columnas esperadas;
- restricciones activas;
- estado final esperado;
- rollback correcto;
- permisos efectivos.

La corrección automática valida el resultado; la rúbrica puede seguir evaluando razonamiento, seguridad y claridad.

## 16. Validación del blueprint

- [x] las 10 UDs están cubiertas;
- [x] diseño conceptual y lógico tienen peso suficiente;
- [x] normalización se evalúa por razonamiento;
- [x] SQL tiene peso principal;
- [x] JOIN y consultas avanzadas tienen evaluación explícita;
- [x] DML contempla seguridad;
- [x] transacciones están representadas;
- [x] mínimo privilegio y backup básico están incluidos;
- [x] D1 no domina el examen;
- [x] examen bajo demanda;
- [x] entorno reproducible y aislado.

## 17. Criterio de salida de ASIR-04

ASIR-04 se considera superado cuando el alumno puede, bajo examen:

- transformar requisitos en un modelo de datos;
- diseñar un ER coherente;
- convertirlo a modelo relacional;
- elegir claves y restricciones;
- detectar y corregir anomalías mediante normalización;
- crear el esquema en SQL;
- modificar datos con seguridad;
- consultar una base de datos con filtros, agregaciones, JOIN y subconsultas;
- utilizar transacciones básicas;
- aplicar privilegios mínimos;
- realizar y comprobar una copia/restauración elemental;
- verificar que el resultado obtenido coincide con lo pedido.

El objetivo no es memorizar SQL, sino comprender los datos y poder diseñarlos, consultarlos y modificarlos de forma correcta y segura.
