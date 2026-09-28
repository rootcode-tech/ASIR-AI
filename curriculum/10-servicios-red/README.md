# ASIR-10 · Servicios de Red e Internet

**Estado:** especificación curricular completada  
**UDs:** 11

## Finalidad

Desplegar, asegurar, operar, monitorizar y diagnosticar los servicios de red fundamentales de una infraestructura moderna.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Arquitectura de servicios, puertos, sockets y resolución de incidencias | Especificada |
| UD02 | DNS autoritativo, recursivo y operación segura | Especificada |
| UD03 | DHCP avanzado, relay y planificación | Especificada |
| UD04 | Servicios web HTTP/HTTPS y servidores web | Especificada |
| UD05 | TLS, certificados, reverse proxy y balanceo básico | Especificada |
| UD06 | Correo electrónico: SMTP, IMAP, autenticación y antispam | Especificada |
| UD07 | Transferencia y acceso: SSH, SFTP y servicios equivalentes | Especificada |
| UD08 | Servicios de archivos: NFS y Samba | Especificada |
| UD09 | VPN, acceso remoto y túneles | Especificada |
| UD10 | Proxy, caché, NTP, syslog y servicios auxiliares | Especificada |
| UD11 | Automatización, monitorización y documentación de servicios | Especificada |

## Arquitectura pedagógica

```text
servicio / puerto / socket
        ↓
DNS
        ↓
DHCP
        ↓
HTTP / web
        ↓
TLS / reverse proxy
        ↓
correo
        ↓
SSH / SFTP
        ↓
NFS / Samba
        ↓
VPN
        ↓
NTP / syslog / proxy
        ↓
automatización + observabilidad + operación integral
```

## Principios

- diagnosticar de proceso a red y de red a aplicación;
- tratar DNS y tiempo como dependencias críticas;
- separar servidor web, reverse proxy y aplicación;
- proteger claves privadas y secretos fuera del repositorio;
- aplicar mínimo privilegio;
- documentar puertos, dependencias y flujos;
- centralizar logs y monitorizar servicios;
- automatizar solo después de comprender la configuración manual;
- versionar configuración reproducible;
- validar siempre con pruebas de aceptación.

## Papel dentro de ASIR-AI

ASIR-10 conecta de forma directa:

- ASIR-02 Redes;
- ASIR-09 Sistemas II;
- ASIR-11 Aplicaciones Web;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps/Cloud;
- ASIR-17 Proyecto.

## Evaluación

Los ejercicios, configuraciones, laboratorios, scripts y runbooks son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se construirán laboratorios de servicios, configuraciones de referencia, escenarios de fallo, blueprints de examen y el desarrollo completo de las 11 UDs.
