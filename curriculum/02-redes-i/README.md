# ASIR-02 · Redes I — Planificación y Administración de Redes

**Estado:** especificación curricular completada  
**UDs:** 10

## Finalidad

Construir una base de redes que permita comprender y diagnosticar comunicaciones reales antes de desplegar servicios, seguridad, cloud o DevOps.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | Modelos OSI/TCP-IP, encapsulación y herramientas de red | Especificada |
| UD02 | Ethernet, direccionamiento MAC, medios y topologías | Especificada |
| UD03 | IPv4, subnetting, VLSM y planificación de direccionamiento | Especificada |
| UD04 | IPv6: direccionamiento, autoconfiguración y coexistencia | Especificada |
| UD05 | Conmutación, STP y fundamentos de switching | Especificada |
| UD06 | VLAN, trunking y segmentación lógica | Especificada |
| UD07 | Routing estático y fundamentos de routing dinámico | Especificada |
| UD08 | DHCP, DNS, NAT/PAT y servicios de apoyo | Especificada |
| UD09 | Redes inalámbricas, seguridad Wi-Fi y movilidad | Especificada |
| UD10 | Captura, diagnóstico, documentación y diseño de una red completa | Especificada |

## Arquitectura pedagógica

```text
capas + herramientas
      ↓
Ethernet
      ↓
IPv4 ─── IPv6
  ↓        ↓
switching/STP
      ↓
VLAN
      ↓
routing
      ↓
DHCP/DNS/NAT
      ↓
Wi-Fi
      ↓
diseño + troubleshooting integral
```

## Principios

- comprender el paquete antes que memorizar comandos;
- separar capa física, enlace, red, transporte y aplicación;
- subnetting razonado, no memorizado;
- IPv6 como protocolo real, no apéndice;
- segmentar con propósito;
- capturar tráfico cuando aporte evidencia;
- documentar topología y direccionamiento;
- diagnosticar desde la capa más baja que pueda explicar el síntoma.

## Relación con módulos posteriores

ASIR-02 es prerrequisito directo de:

- ASIR-09 Sistemas II;
- ASIR-10 Servicios de Red;
- ASIR-11 Aplicaciones Web;
- ASIR-13 Seguridad y Alta Disponibilidad;
- ASIR-16 DevOps, Cloud e IaC;
- ASIR-17 Proyecto.

## Evaluación

Los ejercicios y laboratorios son formativos. La calificación se obtiene mediante exámenes según el blueprint que se diseñará en la fase de evaluación.
