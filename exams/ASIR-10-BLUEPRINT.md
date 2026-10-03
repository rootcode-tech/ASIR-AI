# ASIR-10 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-10 · Servicios de Red e Internet

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica de servicios de red.
- **Modalidad predominante:** despliegue, configuración, validación, seguridad y troubleshooting de servicios.
- **Duración examen final:** 180 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** laboratorio reproducible con varias máquinas virtuales o contenedores y red aislada.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los ejercicios, laboratorios, prácticas de configuración y simulacros previos no generan nota y pueden repetirse sin límite.

## 2. Cálculo de nota

- Exámenes de UD: **60%**
- Examen final integrador: **40%**
- Mínimo examen final: **5,0**
- Mínimo total: **5,0**
- Recuperación: sustituye la nota de la asignatura.
- Sin penalización por retrasar la evaluación.

## 3. Pesos por UD

| UD | Peso dentro del 60% | Justificación |
|---|---:|---|
| UD01 | 7% | Arquitectura de servicios y diagnóstico base. |
| UD02 | 12% | DNS es servicio troncal y dependencia de múltiples capas superiores. |
| UD03 | 8% | DHCP y relay son esenciales para operación de red. |
| UD04 | 12% | HTTP/HTTPS y servidores web son base de publicación de servicios. |
| UD05 | 12% | TLS, certificados, reverse proxy y balanceo son críticos en producción. |
| UD06 | 10% | Correo requiere comprender dependencias, autenticación y seguridad. |
| UD07 | 8% | SSH/SFTP son herramientas esenciales de administración remota. |
| UD08 | 8% | NFS/Samba cubren compartición y permisos en entornos mixtos. |
| UD09 | 8% | VPN y túneles son importantes para acceso remoto seguro. |
| UD10 | 7% | Proxy, caché, NTP y syslog son servicios auxiliares frecuentes. |
| UD11 | 8% | Automatización, monitorización y documentación integran el módulo. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. Arquitectura y resolución | UD01-UD03 | desplegar y validar DNS/DHCP y dependencias | open-lab | D2-D3 | 20 |
| B. Web y publicación segura | UD04-UD05 | servir HTTP/HTTPS, TLS, reverse proxy y validar certificados | open-lab | D2-D4 | 25 |
| C. Correo y acceso remoto | UD06-UD07 | operar correo básico y acceso SSH/SFTP seguro | open-lab | D2-D3 | 15 |
| D. Archivos y acceso remoto seguro | UD08-UD09 | configurar NFS/Samba/VPN y permisos | open-lab | D2-D3 | 15 |
| E. Servicios auxiliares | UD10 | NTP, syslog, proxy/caché y validación | open-lab | D2-D3 | 10 |
| F. Incidente integrador | UD11 + anteriores | diagnosticar una cadena de servicios con fallo compuesto | open-lab | D3-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 5% |
| D2 | Aplicación | 30% |
| D3 | Diagnóstico | 40% |
| D4 | Integración / decisión | 25% |

ASIR-10 debe evaluar operación real de servicios y diagnóstico de dependencias, no memoria de ficheros de configuración.

## 6. Tipos de ítem

Se podrán combinar:

- instalación y configuración de servicios;
- validación de puertos y sockets;
- resolución DNS;
- DHCP y relay;
- HTTP/HTTPS;
- virtual hosts;
- TLS y certificados;
- reverse proxy;
- balanceo básico;
- SMTP/IMAP;
- autenticación y antispam a nivel introductorio;
- SSH/SFTP;
- NFS/Samba;
- VPN/túneles;
- proxy y caché;
- NTP;
- syslog;
- análisis de logs;
- automatización;
- health checks;
- troubleshooting por dependencias.

## 7. Modalidades

### Open-docs

Se permite consultar documentación oficial para:

- sintaxis de configuración;
- parámetros de servicios;
- directivas específicas;
- certificados;
- puertos y opciones;
- formatos de logs.

### Open-lab

Se permite trabajar sobre el entorno, reiniciar servicios, inspeccionar logs y ejecutar pruebas.

El objetivo es demostrar que el alumno puede operar el servicio correctamente y verificarlo.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- exponer un servicio innecesariamente a toda la red;
- desactivar TLS o validación de certificados para “hacer que funcione” sin justificación;
- usar credenciales o secretos inseguros;
- abrir permisos indiscriminados;
- dejar un servicio escuchando donde no debe;
- modificar DNS/DHCP sin verificar impacto;
- afirmar que un servicio funciona solo porque el proceso está activo;
- ignorar logs o dependencias evidentes;
- realizar cambios múltiples sin aislar la causa;
- romper resolución de nombres, autenticación o acceso para corregir otro síntoma;
- desactivar controles de seguridad sin rollback.

## 9. Rúbrica práctica general

| Dimensión | Peso |
|---|---:|
| resultado funcional | 30% |
| configuración correcta | 20% |
| verificación extremo a extremo | 20% |
| seguridad / mínimo privilegio | 15% |
| troubleshooting / razonamiento | 10% |
| documentación | 5% |

## 10. Rúbrica de troubleshooting de servicios

| Dimensión | Peso |
|---|---:|
| definir síntoma y alcance | 10% |
| identificar dependencias | 15% |
| evidencia: estado, socket, log, red | 20% |
| hipótesis | 20% |
| prueba controlada | 15% |
| corrección mínima | 10% |
| validación extremo a extremo / RCA | 10% |

## 11. Exámenes de UD

### UD01

- arquitectura cliente/servidor;
- puertos y sockets;
- dependencias;
- herramientas de diagnóstico.

Modalidad: open-lab.

### UD02

- DNS autoritativo;
- recursión;
- zonas;
- registros;
- resolución directa/inversa;
- caché;
- seguridad operativa.

Modalidad: open-lab.

### UD03

- DHCP;
- scopes;
- reservas;
- opciones;
- relay;
- validación.

Modalidad: open-lab.

### UD04

- HTTP;
- HTTPS;
- servidor web;
- virtual hosts;
- logs;
- publicación.

Modalidad: open-lab.

### UD05

- TLS;
- certificados;
- cadena de confianza;
- reverse proxy;
- balanceo básico;
- validación.

Modalidad: open-lab.

### UD06

- SMTP;
- IMAP;
- autenticación;
- flujo de correo;
- antispam básico;
- diagnóstico.

Modalidad: open-lab controlado.

### UD07

- SSH;
- claves;
- SFTP;
- configuración segura;
- acceso remoto.

Modalidad: open-lab.

### UD08

- NFS;
- Samba;
- exportaciones/recursos;
- permisos;
- acceso desde cliente.

Modalidad: open-lab.

### UD09

- VPN;
- túneles;
- rutas;
- acceso remoto;
- validación y alcance.

Modalidad: open-lab.

### UD10

- proxy;
- caché;
- NTP;
- syslog;
- servicios auxiliares.

Modalidad: open-lab.

### UD11

- automatización de despliegue/configuración básica;
- health checks;
- monitorización;
- documentación;
- troubleshooting integrador.

Modalidad: open-lab integrador.

## 12. Recuperación

La recuperación integral:

- se activa solo cuando el alumno lo solicite;
- utiliza topología y nombres diferentes;
- mantiene dificultad equivalente;
- incluye al menos un fallo DNS o de resolución;
- incluye publicación HTTP/HTTPS;
- incluye un incidente de seguridad o permisos;
- incluye un escenario de troubleshooting compuesto;
- sustituye la nota de ASIR-10;
- no tiene penalización ni límite pedagógico de intentos.

## 13. Requisitos del entorno

El examen deberá poder recrearse automáticamente.

Mínimo recomendado:

- red aislada de laboratorio;
- 3 o más nodos/VM/contenedores;
- servicio DNS;
- DHCP o equivalente simulado;
- servidor web;
- PKI/certificados de laboratorio;
- servicio SSH;
- almacenamiento compartido;
- servicio de logs;
- snapshots o imágenes base;
- scripts para inyectar incidencias.

No se dependerá de dominios, APIs o servicios públicos externos para la parte calificable.

## 14. Principio de verificación

Un servicio no se considera correcto porque:

- “el daemon está running”;
- “el puerto está abierto”;
- “no aparecen errores rojos”.

Debe verificarse extremo a extremo:

1. configuración válida;
2. proceso activo;
3. socket correcto;
4. resolución/ruta disponible;
5. autenticación/permisos correctos;
6. petición real del cliente;
7. respuesta esperada;
8. logs coherentes.

## 15. Validación del blueprint

- [x] las 11 UDs están cubiertas;
- [x] DNS/DHCP tienen evaluación práctica;
- [x] HTTP/HTTPS/TLS tienen peso alto;
- [x] correo está representado;
- [x] SSH/SFTP y archivos están incluidos;
- [x] VPN está incluida;
- [x] NTP/syslog/proxy están representados;
- [x] seguridad y mínimo privilegio son transversales;
- [x] troubleshooting tiene peso explícito;
- [x] entorno reproducible;
- [x] evaluación bajo demanda.

## 16. Criterio de salida de ASIR-10

ASIR-10 se considera superado cuando el alumno puede, bajo examen:

- desplegar y validar DNS y DHCP;
- publicar un servicio web;
- configurar HTTPS correctamente;
- trabajar con certificados;
- usar reverse proxy;
- comprender el flujo básico de correo;
- administrar acceso SSH/SFTP;
- compartir recursos con NFS/Samba;
- configurar acceso remoto mediante VPN/túnel a nivel básico;
- operar NTP/syslog/proxy;
- interpretar logs y dependencias;
- diagnosticar un fallo de servicio de forma estructurada;
- verificar extremo a extremo lo que despliega.

El objetivo es pasar de “instalar servicios” a saber operarlos de forma segura y demostrable.
