# Mapa de dependencias pedagógicas

Este documento define qué conocimientos deben existir antes de introducir tecnologías o bloques posteriores. Su función es impedir que ASIR-AI se convierta en una colección de herramientas sin fundamentos.

## Cadena principal

```text
Acceso / fundamentos
        ↓
Hardware + Sistemas I + Redes I
        ↓
Linux/Windows operativos + TCP/IP + almacenamiento
        ↓
Bases de datos + formatos de datos + documentación
        ↓
Sistemas II + Servicios de red
        ↓
Aplicaciones web + Administración de SGBD
        ↓
Seguridad y alta disponibilidad
        ↓
Docker / CI-CD / Ansible / Terraform / Cloud
        ↓
Kubernetes introductorio + Observabilidad / SRE
        ↓
Proyecto ASIR-AI
```

## Dependencias clave

| Tecnología / competencia | No introducir a fondo antes de | Introducción | Consolidación |
|---|---|---|---|
| Git y GitHub | manejo básico de ficheros y Markdown | ASIR-05 UD09 + prácticas iniciales | ASIR-16 UD01 y proyecto |
| GNU/Linux | fundamentos de SO | ASIR-01 UD05 | ASIR-09 UD01 y ASIR-16 UD02 |
| Bash | terminal Linux, permisos y procesos | ASIR-01 | ASIR-09 UD06-07 |
| PowerShell | Windows y shell básica | ASIR-01 UD08 | ASIR-09 UD02/UD06 |
| Python | lógica básica, terminal y ficheros | transversal tras ASIR-01/05 | automatización en ASIR-09/16 |
| SQL | modelo relacional | ASIR-04 | ASIR-12 |
| HTTP/APIs | redes + formatos estructurados | ASIR-05 UD07 | ASIR-10/11 |
| TLS/PKI | TCP/IP + servicios + identidad | ASIR-10 UD05 | ASIR-13 UD03 |
| Docker | procesos, redes, filesystem y servicios | ASIR-09 UD08 | ASIR-11 UD05 y ASIR-16 UD03-04 |
| CI/CD | Git + despliegue manual | ASIR-11 UD08 | ASIR-16 UD05 |
| Ansible | administración manual + SSH + YAML | ASIR-16 UD06 | proyecto |
| Terraform | redes + cloud conceptual + Git | ASIR-16 UD07 | proyecto |
| Cloud | sistemas, redes, IAM conceptual | ASIR-07 UD04 | ASIR-16 UD08 |
| Kubernetes | Docker + redes + YAML + servicios | ASIR-16 UD09 | nivel introductorio |
| Observabilidad | logs + servicios + métricas | ASIR-09 UD10 | ASIR-11 UD10 / ASIR-16 UD10 |
| IA aplicada | competencia digital y verificación | ASIR-07 UD06 | uso transversal controlado |
| Seguridad | sistemas y redes básicos | transversal desde primero | ASIR-13 |

## Regla de profundidad

Una tecnología puede **aparecer** antes para dar contexto, pero no se evaluará operativamente hasta que estén cubiertos sus prerrequisitos.

## Manual antes que automatizado

Para cualquier operación crítica se seguirá esta secuencia:

1. comprender el componente;
2. ejecutarlo manualmente;
3. verificar el resultado;
4. provocar y diagnosticar fallos;
5. documentarlo;
6. automatizarlo;
7. observar y mantener la automatización.

Esta regla es especialmente importante para Ansible, Terraform, CI/CD y herramientas asistidas por IA.
