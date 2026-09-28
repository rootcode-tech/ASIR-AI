# ASIR-11 · Web e Infraestructura — Implantación de Aplicaciones Web

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Desplegar, publicar, mantener, proteger, automatizar y observar aplicaciones web modernas entendiendo todas sus dependencias de infraestructura.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Arquitectura web, HTTP y componentes de una aplicación | Especificada |
| UD02 | Servidores web, virtual hosts y runtime de aplicaciones | Especificada |
| UD03 | Despliegue de aplicaciones con base de datos | Especificada |
| UD04 | CMS y plataformas web: instalación, actualización y operación | Especificada |
| UD05 | Contenedores para aplicaciones web | Especificada |
| UD06 | Reverse proxy, TLS, dominios y publicación segura | Especificada |
| UD07 | Configuración, secretos y entornos de despliegue | Especificada |
| UD08 | CI/CD introductorio para despliegues | Especificada |
| UD09 | Seguridad, backups y mantenimiento de aplicaciones | Especificada |
| UD10 | Observabilidad, pruebas y proyecto de despliegue completo | Especificada |

## Arquitectura pedagógica

```text
arquitectura web / HTTP
        ↓
web server / runtime
        ↓
aplicación + base de datos
        ↓
CMS / plataformas
        ↓
contenedores
        ↓
reverse proxy / TLS / DNS
        ↓
configuración / secretos / entornos
        ↓
CI/CD
        ↓
seguridad / backups / mantenimiento
        ↓
observabilidad + despliegue integral
```

## Principios

- comprender la arquitectura antes de automatizar;
- separar servidor web, runtime, aplicación y base de datos;
- aplicar mínimo privilegio;
- no versionar secretos;
- usar staging antes de producción;
- desplegar con rollback;
- integrar backup y restore en el ciclo de vida;
- observar logs, métricas y health checks;
- validar mediante pruebas de aceptación;
- considerar un despliegue completo solo si es reproducible, seguro, observable y recuperable.

## Papel dentro de ASIR-AI

ASIR-11 conecta directamente:

- ASIR-04 Bases de Datos I;
- ASIR-05 Lenguajes y Datos;
- ASIR-09 Sistemas II;
- ASIR-10 Servicios de Red;
- ASIR-12 Administración de SGBD;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps/Cloud;
- ASIR-17 Proyecto.

Los contenedores y CI/CD se introducen aquí de forma aplicada al despliegue web; su tratamiento profesional y transversal se profundizará en ASIR-16.

## Evaluación

Los ejercicios, despliegues, pipelines, backups, incidentes y documentación son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se crearán laboratorios completos, aplicaciones de práctica, pipelines, escenarios de fallo, blueprints de examen y las lecciones completas de las 10 UDs.
