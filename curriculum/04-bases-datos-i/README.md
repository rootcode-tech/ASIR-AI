# ASIR-04 · Bases de Datos I — Gestión de Bases de Datos

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Diseñar bases de datos relacionales correctas y operar SQL con integridad, transacciones, seguridad básica y procedimientos de copia/restauración.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Sistemas de información y modelos de datos | Especificada |
| UD02 | Modelo entidad-relación y diseño conceptual | Especificada |
| UD03 | Modelo relacional, claves y restricciones | Especificada |
| UD04 | Normalización y calidad del diseño | Especificada |
| UD05 | SQL DDL: esquemas, tablas, tipos y restricciones | Especificada |
| UD06 | SQL DML: inserción, actualización y borrado | Especificada |
| UD07 | Consultas SELECT, funciones, agregación y ordenación | Especificada |
| UD08 | JOIN, subconsultas, vistas y consultas avanzadas | Especificada |
| UD09 | Transacciones, concurrencia e integridad | Especificada |
| UD10 | Usuarios, privilegios, copias y operación básica del SGBD | Especificada |

## Arquitectura pedagógica

```text
sistemas de información
        ↓
modelo ER
        ↓
modelo relacional
        ↓
normalización
        ↓
DDL
        ↓
DML
        ↓
SELECT / agregación
        ↓
JOIN / subconsultas / vistas
        ↓
transacciones / concurrencia
        ↓
roles / backup / restore
```

## SGBD de referencia

- PostgreSQL como plataforma principal.
- MariaDB/MySQL como contraste cuando aporte valor.
- SQL estándar como referencia conceptual siempre que sea posible.

Las versiones concretas se fijarán al comenzar el curso.

## Principios

- diseñar antes de implementar;
- imponer integridad en la base cuando corresponda;
- normalizar con criterio, no mecánicamente;
- verificar con SELECT antes de UPDATE/DELETE;
- usar transacciones para cambios sensibles;
- aplicar mínimo privilegio;
- versionar scripts SQL;
- probar la restauración de los backups.

## Relación con módulos posteriores

ASIR-04 es base directa de:

- ASIR-11 Implantación de Aplicaciones Web;
- ASIR-12 Administración de SGBD;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 automatización y plataformas;
- ASIR-17 Proyecto.

## Evaluación

Los ejercicios y laboratorios son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se desarrollarán bancos de ejercicios, datasets, laboratorios reproducibles, blueprints de examen y las lecciones completas de cada UD.
