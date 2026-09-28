# Currículo Maestro ASIR-AI

**Versión:** 0.3.0-draft  
**Estado:** 172 UDs especificadas; auditoría estructural y pedagógica v0.3 completada  
**Marca:** RootCode Technologies

## Propósito

Definir el recorrido completo antes de impartir ninguna clase. Este documento fija la secuencia de las 18 asignaturas, sus 172 unidades didácticas y las dependencias pedagógicas. Las 172 UDs ya cuentan con especificación curricular; el currículo permanece en borrador hasta completar evaluación, carga, laboratorios, proyecto y auditoría final v1.0.

## Contrato pedagógico de cada UD

Cada unidad se desarrollará con: **objetivos → conocimientos previos → contenidos → teoría → herramientas → ejercicios → laboratorio → documentación/entregables → competencias transversales → criterios de dominio → preparación del examen → examen**.

## Reglas de progresión

- No introducir una tecnología antes de cubrir sus fundamentos.
- Evitar duplicación: una materia se enseña a fondo en su módulo de origen y se reutiliza en los demás.
- Primero operación manual y comprensión; después automatización.
- Primero sistemas y redes; después contenedores, IaC, cloud y orquestación.
- Git y documentación se introducen pronto y se usan durante todo el ciclo.
- Los ejercicios y laboratorios son formativos; la calificación se obtiene mediante exámenes.

## Mapa global

### ASIR-00 · Preparación de acceso a Grado Superior

**Propósito:** Preparar la prueba de acceso con un enfoque aplicado a informática, construyendo la base matemática, lingüística, científica, inglesa y digital necesaria para afrontar ASIR.

**Prerrequisitos:** Ninguno; diagnóstico inicial obligatorio.

- **UD01 — Diagnóstico, método de estudio y razonamiento técnico**
- **UD02 — Aritmética, proporcionalidad, porcentajes y notación científica**
- **UD03 — Álgebra: expresiones, ecuaciones, sistemas e inecuaciones**
- **UD04 — Funciones, gráficas y modelización**
- **UD05 — Geometría, trigonometría y medida**
- **UD06 — Estadística, probabilidad e interpretación de datos**
- **UD07 — Fundamentos científico-tecnológicos aplicados**
- **UD08 — Lengua: comprensión, síntesis y expresión escrita**
- **UD09 — Inglés funcional y competencia digital**
- **UD10 — Estrategia de examen y simulacros integrales**

### ASIR-01 · Sistemas I — Implantación de Sistemas Operativos

**Propósito:** Instalar, configurar, operar y diagnosticar sistemas operativos cliente y servidor, con especial atención a GNU/Linux y Windows.

**Prerrequisitos:** ASIR-00 recomendado.

- **UD01 — Arquitectura de computadores y fundamentos de sistemas operativos**
- **UD02 — Virtualización de laboratorio y gestión de máquinas virtuales**
- **UD03 — Instalación, arranque, particionado y despliegue de sistemas**
- **UD04 — Sistemas de archivos, montaje y jerarquía del sistema**
- **UD05 — Terminal GNU/Linux y administración básica**
- **UD06 — Usuarios, grupos, permisos, ACL y privilegios**
- **UD07 — Procesos, servicios, arranque, paquetes y registros**
- **UD08 — Administración básica de Windows y PowerShell**
- **UD09 — Almacenamiento, copias de seguridad y recuperación básica**
- **UD10 — Mantenimiento, diagnóstico y resolución estructurada de incidencias**

### ASIR-02 · Redes I — Planificación y Administración de Redes

**Propósito:** Comprender, diseñar, configurar y diagnosticar redes IP desde la capa física hasta el encaminamiento y los servicios básicos.

**Prerrequisitos:** ASIR-00; coordinación estrecha con ASIR-01 y ASIR-03.

- **UD01 — Modelos OSI/TCP-IP, encapsulación y herramientas de red**
- **UD02 — Ethernet, direccionamiento MAC, medios y topologías**
- **UD03 — IPv4, subnetting, VLSM y planificación de direccionamiento**
- **UD04 — IPv6: direccionamiento, autoconfiguración y coexistencia**
- **UD05 — Conmutación, STP y fundamentos de switching**
- **UD06 — VLAN, trunking y segmentación lógica**
- **UD07 — Routing estático y fundamentos de routing dinámico**
- **UD08 — DHCP, DNS, NAT/PAT y servicios de apoyo**
- **UD09 — Redes inalámbricas, seguridad Wi-Fi y movilidad**
- **UD10 — Captura, diagnóstico, documentación y diseño de una red completa**

### ASIR-03 · Hardware y CPD — Fundamentos de Hardware

**Propósito:** Seleccionar, montar, mantener y diagnosticar hardware de puesto, servidor y CPD entendiendo disponibilidad, energía, almacenamiento y ciclo de vida.

**Prerrequisitos:** ASIR-00 recomendado.

- **UD01 — Arquitectura de hardware: CPU, memoria, buses y placas**
- **UD02 — UEFI/BIOS, POST, arranque y configuración de firmware**
- **UD03 — Almacenamiento: HDD, SSD, NVMe e interfaces**
- **UD04 — RAID, redundancia y rendimiento de almacenamiento**
- **UD05 — Hardware de servidor, gestión remota y componentes empresariales**
- **UD06 — Energía, fuentes, UPS, protección y continuidad**
- **UD07 — Racks, cableado, refrigeración y fundamentos de CPD**
- **UD08 — Dispositivos de red, periféricos y compatibilidad**
- **UD09 — Diagnóstico, mantenimiento, inventario y ciclo de vida**

### ASIR-04 · Bases de Datos I — Gestión de Bases de Datos

**Propósito:** Diseñar bases de datos relacionales correctas y operar SQL con integridad, transacciones y seguridad básica.

**Prerrequisitos:** Competencia matemática y lógica básica; ASIR-00 recomendado.

- **UD01 — Sistemas de información y modelos de datos**
- **UD02 — Modelo entidad-relación y diseño conceptual**
- **UD03 — Modelo relacional, claves y restricciones**
- **UD04 — Normalización y calidad del diseño**
- **UD05 — SQL DDL: esquemas, tablas, tipos y restricciones**
- **UD06 — SQL DML: inserción, actualización y borrado**
- **UD07 — Consultas SELECT, funciones, agregación y ordenación**
- **UD08 — JOIN, subconsultas, vistas y consultas avanzadas**
- **UD09 — Transacciones, concurrencia e integridad**
- **UD10 — Usuarios, privilegios, copias y operación básica del SGBD**

### ASIR-05 · Lenguajes y Datos — Lenguajes de Marcas y SGI

**Propósito:** Representar, validar, transformar e intercambiar información estructurada en formatos usados por sistemas, aplicaciones y automatización.

**Prerrequisitos:** Competencia digital básica.

- **UD01 — HTML semántico y estructura de documentos**
- **UD02 — CSS esencial y presentación accesible**
- **UD03 — XML bien formado, namespaces y modelos de documento**
- **UD04 — DTD, XML Schema y validación**
- **UD05 — XPath y transformación con XSLT**
- **UD06 — JSON, YAML, TOML y formatos de configuración**
- **UD07 — APIs, HTTP y representación de datos**
- **UD08 — Sindicación, intercambio e integración de información**
- **UD09 — Documentación técnica con Markdown y automatización de datos**

### ASIR-06 · Carrera Profesional I — IPE I

**Propósito:** Comprender el entorno laboral, los derechos y obligaciones profesionales, la prevención y las competencias personales necesarias para incorporarse al sector.

**Prerrequisitos:** Ninguno.

- **UD01 — Sector IT, perfiles profesionales y competencias**
- **UD02 — Relaciones laborales, derechos y deberes**
- **UD03 — Contratación, nómina y Seguridad Social**
- **UD04 — Prevención de riesgos laborales y cultura preventiva**
- **UD05 — Emergencias, primeros auxilios y actuación segura**
- **UD06 — Comunicación profesional, equipo y resolución de conflictos**
- **UD07 — Empleabilidad, aprendizaje continuo e identidad digital**
- **UD08 — Plan profesional personal y evidencias de competencia**

### ASIR-07 · Transformación Digital — Digitalización

**Propósito:** Entender cómo datos, cloud, automatización, IA, seguridad y plataformas digitales transforman procesos y organizaciones.

**Prerrequisitos:** Competencia digital básica.

- **UD01 — Transformación digital, procesos y madurez tecnológica**
- **UD02 — Sistemas IT/OT, conectividad y plataformas**
- **UD03 — Datos, analítica y gobierno de la información**
- **UD04 — Cloud, edge y modelos de servicio**
- **UD05 — Automatización, integración y APIs**
- **UD06 — IA, modelos generativos y uso profesional responsable**
- **UD07 — Ciberseguridad, privacidad, ética y riesgo digital**
- **UD08 — Proyecto de digitalización de un proceso real**

### ASIR-08 · Tecnología Sostenible — Sostenibilidad

**Propósito:** Aplicar criterios ambientales, sociales y de eficiencia al ciclo de vida de la infraestructura tecnológica.

**Prerrequisitos:** Ninguno.

- **UD01 — Sostenibilidad, ODS, ESG y marco profesional**
- **UD02 — Impacto ambiental del hardware y ciclo de vida**
- **UD03 — Consumo energético, eficiencia y medición**
- **UD04 — Residuos electrónicos, reutilización y economía circular**
- **UD05 — Compra tecnológica responsable y cadena de suministro**
- **UD06 — CPD, cloud y Green IT**
- **UD07 — Indicadores, huella y mejora continua**
- **UD08 — Plan de sostenibilidad para una infraestructura IT**

### ASIR-09 · Sistemas II — Administración de Sistemas Operativos

**Propósito:** Administrar de forma avanzada sistemas Linux y Windows, identidades, almacenamiento, automatización, copias, monitorización y endurecimiento.

**Prerrequisitos:** ASIR-01, ASIR-02 y ASIR-03.

- **UD01 — Administración avanzada de GNU/Linux**
- **UD02 — Windows Server y administración remota**
- **UD03 — Active Directory, dominios y políticas de grupo**
- **UD04 — Identidad, LDAP, Kerberos y servicios de directorio**
- **UD05 — LVM, RAID software, cuotas y almacenamiento avanzado**
- **UD06 — Automatización con Bash y PowerShell**
- **UD07 — Tareas programadas, systemd timers y operación repetible**
- **UD08 — Virtualización avanzada y fundamentos de contenedores**
- **UD09 — Backups, restauración y recuperación ante fallos**
- **UD10 — Logs, monitorización, auditoría y observabilidad básica**
- **UD11 — Hardening, mantenimiento y troubleshooting avanzado**

### ASIR-10 · Servicios de Red e Internet

**Propósito:** Desplegar y operar servicios de infraestructura y de Internet de forma segura, documentada y observable.

**Prerrequisitos:** ASIR-01 y ASIR-02; ASIR-09 en paralelo.

- **UD01 — Arquitectura de servicios, puertos, sockets y resolución de incidencias**
- **UD02 — DNS autoritativo, recursivo y operación segura**
- **UD03 — DHCP avanzado, relay y planificación**
- **UD04 — Servicios web HTTP/HTTPS y servidores web**
- **UD05 — TLS, certificados, reverse proxy y balanceo básico**
- **UD06 — Correo electrónico: SMTP, IMAP, autenticación y antispam**
- **UD07 — Transferencia y acceso: SSH, SFTP y servicios equivalentes**
- **UD08 — Servicios de archivos: NFS y Samba**
- **UD09 — VPN, acceso remoto y túneles**
- **UD10 — Proxy, caché, NTP, syslog y servicios auxiliares**
- **UD11 — Automatización, monitorización y documentación de servicios**

### ASIR-11 · Web e Infraestructura — Implantación de Aplicaciones Web

**Propósito:** Desplegar aplicaciones web sobre una infraestructura reproducible, segura y mantenible.

**Prerrequisitos:** ASIR-01, ASIR-04, ASIR-05 y fundamentos de ASIR-10.

- **UD01 — Arquitectura web, HTTP y componentes de una aplicación**
- **UD02 — Servidores web, virtual hosts y runtime de aplicaciones**
- **UD03 — Despliegue de aplicaciones con base de datos**
- **UD04 — CMS y plataformas web: instalación, actualización y operación**
- **UD05 — Contenedores para aplicaciones web**
- **UD06 — Reverse proxy, TLS, dominios y publicación segura**
- **UD07 — Configuración, secretos y entornos de despliegue**
- **UD08 — CI/CD introductorio para despliegues**
- **UD09 — Seguridad, backups y mantenimiento de aplicaciones**
- **UD10 — Observabilidad, pruebas y proyecto de despliegue completo**

### ASIR-12 · Bases de Datos II — Administración de SGBD

**Propósito:** Administrar SGBD en producción atendiendo a seguridad, rendimiento, recuperación, replicación, disponibilidad y automatización.

**Prerrequisitos:** ASIR-04 y fundamentos de ASIR-09.

- **UD01 — Arquitectura interna y ciclo de vida de un SGBD**
- **UD02 — Instalación, configuración y gestión de instancias**
- **UD03 — Usuarios, roles, privilegios y separación de funciones**
- **UD04 — Almacenamiento físico, índices y mantenimiento**
- **UD05 — Transacciones, bloqueos, concurrencia y aislamiento**
- **UD06 — Optimización de consultas y análisis de rendimiento**
- **UD07 — Backup, restore y recuperación punto en el tiempo**
- **UD08 — Replicación, alta disponibilidad y continuidad**
- **UD09 — Auditoría, cifrado y hardening del SGBD**
- **UD10 — Automatización, monitorización y troubleshooting**

### ASIR-13 · Ciberseguridad y Alta Disponibilidad

**Propósito:** Diseñar y operar infraestructura segura y resiliente mediante controles preventivos, detección, respuesta, continuidad y alta disponibilidad.

**Prerrequisitos:** ASIR-02, ASIR-09, ASIR-10 y ASIR-12 en paralelo.

- **UD01 — Riesgo, amenazas, vulnerabilidades y modelo de defensa**
- **UD02 — Hardening de sistemas y gestión de configuración segura**
- **UD03 — Identidad, MFA, PKI, certificados y gestión de secretos**
- **UD04 — Firewalls, segmentación, ACL y Zero Trust introductorio**
- **UD05 — IDS/IPS, EDR y fundamentos de SIEM**
- **UD06 — Gestión de vulnerabilidades y parcheado**
- **UD07 — Seguridad de servicios web, red y aplicaciones**
- **UD08 — Copias, recuperación y continuidad de negocio**
- **UD09 — Alta disponibilidad, clustering y balanceo**
- **UD10 — Respuesta a incidentes, evidencias y forense básico**
- **UD11 — Cumplimiento, privacidad, políticas y auditoría**
- **UD12 — Laboratorio integral de seguridad y resiliencia**

### ASIR-14 · Inglés Profesional IT

**Propósito:** Comprender documentación técnica y comunicarse con precisión en situaciones habituales de soporte, administración y trabajo internacional.

**Prerrequisitos:** Nivel básico de inglés; ASIR-00 UD09 recomendado.

- **UD01 — Terminología de sistemas, redes y hardware**
- **UD02 — Lectura de documentación, RFC, manuales y changelogs**
- **UD03 — Tickets, incidencias y comunicación de soporte**
- **UD04 — Correo, informes y documentación técnica**
- **UD05 — Reuniones, handover y comunicación oral**
- **UD06 — CV, perfil profesional y entrevista técnica**
- **UD07 — Cloud, DevOps y seguridad en documentación inglesa**
- **UD08 — Presentación técnica final en inglés**

### ASIR-15 · Carrera Profesional II — IPE II

**Propósito:** Convertir las competencias técnicas en una estrategia profesional: empleo, portfolio, proyectos, emprendimiento y presentación de valor.

**Prerrequisitos:** ASIR-06.

- **UD01 — Mapa profesional, especialización y estrategia de carrera**
- **UD02 — Búsqueda de empleo, networking y canales profesionales**
- **UD03 — Portfolio técnico, GitHub y evidencias verificables**
- **UD04 — CV, carta, entrevista y prueba técnica**
- **UD05 — Emprendimiento, propuesta de valor y modelo de negocio**
- **UD06 — Costes, precios, viabilidad y finanzas básicas**
- **UD07 — Gestión de proyectos, Agile/Kanban y trabajo profesional**
- **UD08 — Plan de inserción profesional y defensa del perfil**

### ASIR-16 · Especialización — DevOps, Cloud e IA para Sistemas

**Propósito:** Integrar herramientas modernas de automatización e infraestructura como código sobre una base sólida de sistemas y redes.

**Prerrequisitos:** ASIR-01, ASIR-02, ASIR-05, ASIR-09 y fundamentos de ASIR-10/11.

- **UD01 — Flujo profesional con Git, ramas, PR, releases y SemVer**
- **UD02 — Linux para DevOps y automatización reproducible**
- **UD03 — Docker: imágenes, contenedores, redes y volúmenes**
- **UD04 — Docker Compose y stacks multi-servicio**
- **UD05 — CI/CD con pipelines y quality gates**
- **UD06 — Ansible: inventarios, playbooks, roles e idempotencia**
- **UD07 — Terraform e Infrastructure as Code**
- **UD08 — Cloud: IAM, redes, compute, storage y costes**
- **UD09 — Kubernetes: arquitectura y operación introductoria**
- **UD10 — Observabilidad, SRE, IA asistida y proyecto DevOps**

### ASIR-17 · Proyecto ASIR-AI

**Propósito:** Integrar sistemas, redes, datos, servicios, seguridad, automatización y documentación en una infraestructura empresarial reproducible.

**Prerrequisitos:** Se alimenta de todo el ciclo; ejecución principal tras consolidar módulos técnicos de segundo.

- **UD01 — Problema, requisitos, alcance y criterios de aceptación**
- **UD02 — Arquitectura, ADR y diseño de red/servicios**
- **UD03 — Repositorio, Git, documentación e Infrastructure as Code**
- **UD04 — Plataforma base: red, sistemas, identidad y almacenamiento**
- **UD05 — Servicios de infraestructura y publicación**
- **UD06 — Datos, aplicaciones y persistencia**
- **UD07 — Seguridad, alta disponibilidad y continuidad**
- **UD08 — Automatización, CI/CD y despliegue reproducible**
- **UD09 — Observabilidad, backups, pruebas y recuperación**
- **UD10 — Validación final, memoria, portfolio y defensa**

## Puertas de control

Estado tras auditoría v0.3:

- estructura: ✅ 18 asignaturas / 172 UDs;
- especificación de UDs: ✅;
- dependencias y progresión transversal: ✅ auditadas;
- solapamientos principales: ✅ clasificados como progresión deliberada;
- alineación oficial a nivel de módulos: ✅ documentada en `docs/OFFICIAL_ALIGNMENT.md`;
- matriz oficial RA/CE → UDs: ⏳;
- carga y temporalización: ⏳;
- diseño completo de evaluación: ⏳;
- laboratorios y ejercicios reproducibles: ⏳;
- proyecto integrador detallado por hitos: ⏳;
- auditoría final Curriculum Master v1.0: ⏳.

La auditoría global se documenta en `docs/CURRICULUM_AUDIT_v0.3.md`.

## Siguiente fase

**Fase 4 — Diseño de evaluación.**

Se definirán blueprints de examen, cobertura, dificultad, tipos de ítems, bancos de preguntas y exámenes finales por asignatura. Después se abordarán carga/temporalización, laboratorios y ejercicios, proyecto integrador y auditoría v1.0.
