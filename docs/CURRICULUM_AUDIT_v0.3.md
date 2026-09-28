# Auditoría global del currículo ASIR-AI — v0.3

**Fecha:** 2026-09-28  
**Estado:** auditoría estructural y pedagógica completada  
**Alcance:** mapa maestro, 18 asignaturas, 172 UDs, dependencias, progresión transversal, solapamientos y alineación oficial a nivel de módulos.

## 1. Resultado ejecutivo

El diseño curricular es coherente y puede avanzar a la fase de evaluación.

Se han verificado:

- 18 carpetas de asignatura;
- 18 README de asignatura;
- 172 archivos UDxx.md;
- nomenclatura estable ASIR-00 ... ASIR-17;
- progresión técnica desde fundamentos hasta proyecto;
- separación razonable entre introducción, práctica, consolidación y aplicación profesional;
- política de evaluación consistente: ejercicios y laboratorios formativos; exámenes calificables;
- integración transversal de Git, documentación, seguridad, automatización, cloud, observabilidad e IA.

No se detectan huecos estructurales que obliguen a rediseñar el mapa de 172 UDs.

## 2. Correcciones realizadas durante la auditoría

### 2.1 Dependencias circulares o ambiguas

Se corrigieron tres referencias:

- ASIR-09 UD04 ya no recomienda ASIR-10 como prerrequisito de DNS; utiliza ASIR-02 UD08.
- ASIR-12 UD08 ya no depende contextualmente de ASIR-13; utiliza fundamentos previos de disponibilidad/balanceo.
- ASIR-12 UD09 ya no recomienda ASIR-13 como fundamento de seguridad; utiliza ASIR-07 y ASIR-09.

Resultado: la cadena principal de prerrequisitos queda acíclica.

### 2.2 Python

Python figuraba en el roadmap transversal pero su consolidación no era suficientemente explícita.

Se fija ahora:

- introducción contextual: ASIR-05 UD09;
- práctica: pequeñas utilidades;
- consolidación: ASIR-16 UD02 y UD10;
- aplicación profesional: ASIR-17 cuando aporte valor.

No se crea una asignatura específica de programación: Python se utiliza como herramienta de automatización para un perfil ASIR.

### 2.3 Metadatos

`curriculum/curriculum.yml` se sincroniza con el estado real:

- versión 0.3.0-draft;
- estado global `specification-complete-audited`;
- las 172 UDs pasan de `planned` a `specified`.

## 3. Revisión de progresión pedagógica

Cadena validada:

```text
Acceso
  ↓
Hardware + Sistemas I + Redes I
  ↓
Bases de datos + formatos + documentación
  ↓
Sistemas II + Servicios
  ↓
Aplicaciones web + Administración SGBD
  ↓
Seguridad + Alta disponibilidad
  ↓
Git profesional + Docker + CI/CD
  ↓
Ansible + Terraform + Cloud
  ↓
Kubernetes introductorio + Observabilidad/SRE
  ↓
Proyecto ASIR-AI
```

### Resultado

No se detecta ninguna tecnología principal evaluada operativamente antes de sus fundamentos.

## 4. Revisión de solapamientos

Los solapamientos encontrados son deliberados y forman una progresión de profundidad.

| Área | Introducción | Aplicación / consolidación | Integración |
|---|---|---|---|
| Git | ASIR-05 | ASIR-16 | ASIR-17 |
| Linux | ASIR-01 | ASIR-09 / ASIR-16 | ASIR-17 |
| DNS/DHCP | ASIR-02 | ASIR-10 | ASIR-17 |
| TLS/PKI | ASIR-10 | ASIR-13 | ASIR-17 |
| Backups | ASIR-01 | ASIR-09/11/12/13 | ASIR-17 |
| Docker | ASIR-09 | ASIR-11 / ASIR-16 | ASIR-17 |
| CI/CD | ASIR-11 | ASIR-16 | ASIR-17 |
| Seguridad | ASIR-01/02 | ASIR-13 | ASIR-17 |
| Observabilidad | ASIR-09 | ASIR-10/11/12/16 | ASIR-17 |
| Cloud | ASIR-07 | ASIR-16 | ASIR-17 |
| IA | ASIR-07 | uso transversal / ASIR-16 | ASIR-17 |

Regla editorial para el desarrollo futuro: el módulo posterior reutiliza y amplía; no vuelve a impartir desde cero la teoría del módulo de origen.

## 5. Revisión de coherencia del proyecto final

ASIR-17 está correctamente situado después de la consolidación técnica.

La arquitectura del proyecto exige trazabilidad:

```text
requisito
  ↓
decisión / ADR
  ↓
implementación
  ↓
prueba
  ↓
evidencia
  ↓
operación / recuperación
```

No se obliga a utilizar Docker, Kubernetes, Terraform, cloud u otra tecnología si no existe una necesidad arquitectónica justificable.

## 6. Alineación oficial

La correspondencia a nivel de módulos se documenta en:

- `docs/OFFICIAL_ALIGNMENT.md`

Conclusión de esta auditoría:

- ASIR-01 ... ASIR-15 y ASIR-17 cubren los módulos oficiales nominativos del ciclo actual.
- ASIR-16 es ampliación moderna ASIR-AI y puede servir como marco para la optativa, sin afirmar equivalencia administrativa automática.
- ASIR-00 es preparación previa y no pertenece al ciclo oficial.
- La formación en empresa es un requisito del sistema oficial y no se sustituye con este repositorio.

## 7. Gates todavía abiertos antes de v1.0

La auditoría no congela aún el currículo maestro.

Quedan pendientes:

1. **Matriz RA/CE oficial → UDs.** Verificar resultados de aprendizaje y criterios de evaluación contra normativa vigente.
2. **Diseño de evaluación.** Blueprints, dificultad, cobertura, bancos y exámenes finales.
3. **Carga y temporalización.** Estimar horas por UD y comprobar equilibrio por asignatura.
4. **Laboratorios y ejercicios.** Diseñar prácticas reproducibles con prerequisitos, validación y rollback.
5. **Proyecto integrador.** Convertir ASIR-17 en hitos ejecutables y criterios de aceptación detallados.
6. **Auditoría v1.0 final.** Cobertura, carga, duplicidad residual y coherencia global.

## 8. Decisión de auditoría

**APTO PARA PASAR A FASE 4 — DISEÑO DE EVALUACIÓN.**

No se inicia todavía el estudio de las UDs. La regla de AGENTS.md se mantiene hasta Curriculum Master v1.0.
