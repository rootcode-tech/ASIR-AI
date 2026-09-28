# ASIR-05 · Lenguajes y Datos — Lenguajes de Marcas y SGI

**Estado:** especificación curricular completada  
**UDs:** 9

## Finalidad

Representar, validar, transformar, intercambiar y documentar información estructurada mediante formatos y protocolos utilizados en sistemas, aplicaciones y automatización.

## Secuencia

| UD | Título | Estado |
|---|---|---|
| UD01 | HTML semántico y estructura de documentos | Especificada |
| UD02 | CSS esencial y presentación accesible | Especificada |
| UD03 | XML bien formado, namespaces y modelos de documento | Especificada |
| UD04 | DTD, XML Schema y validación | Especificada |
| UD05 | XPath y transformación con XSLT | Especificada |
| UD06 | JSON, YAML, TOML y formatos de configuración | Especificada |
| UD07 | APIs, HTTP y representación de datos | Especificada |
| UD08 | Sindicación, intercambio e integración de información | Especificada |
| UD09 | Documentación técnica con Markdown y automatización de datos | Especificada |

## Arquitectura pedagógica

```text
HTML
 ↓
CSS
 ↓
XML
 ↓
DTD / XSD
 ↓
XPath / XSLT
 ↓
JSON / YAML / TOML
 ↓
HTTP / APIs
 ↓
integración
 ↓
Markdown + Git + automatización
```

## Principios

- separar estructura, presentación y significado;
- validar datos cuando exista contrato;
- entender formatos antes de automatizarlos;
- tratar APIs como contratos entre sistemas;
- versionar documentación y configuraciones;
- no guardar secretos en repositorios;
- usar Git y Markdown como herramientas permanentes a partir de esta asignatura;
- priorizar formatos y conceptos transferibles frente a herramientas concretas.

## Papel transversal

ASIR-05 es el punto donde Git, GitHub y Markdown pasan de ser una introducción a formar parte del flujo habitual de ASIR-AI.

También prepara directamente para:

- configuración YAML/TOML de herramientas;
- consumo de APIs;
- automatización con scripts;
- Docker/Compose;
- Ansible;
- Terraform;
- CI/CD;
- documentación del proyecto final.

## Relación con módulos posteriores

ASIR-05 alimenta directamente:

- ASIR-10 Servicios de Red;
- ASIR-11 Aplicaciones Web;
- ASIR-16 DevOps, Cloud e IA;
- ASIR-17 Proyecto.

## Evaluación

Los ejercicios y laboratorios son formativos. La calificación se obtiene mediante exámenes.

## Estado de cierre

La asignatura queda curricularmente especificada. En fases posteriores se desarrollarán ejercicios, laboratorios, datasets, prácticas de API, blueprints de evaluación y las lecciones completas de cada UD.
