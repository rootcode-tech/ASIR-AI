# ASIR-05 · Blueprint de evaluación

**Versión:** 0.1.0  
**Estado:** aprobado  
**Asignatura:** ASIR-05 · Lenguajes y Datos — Lenguajes de Marcas y SGI

## 1. Perfil de evaluación

- **Tipo de asignatura:** técnica de representación, validación, transformación e intercambio de información.
- **Modalidad predominante:** edición, validación, transformación, interpretación y documentación.
- **Duración examen final:** 150 minutos orientativos.
- **Recursos permitidos:** open-docs y open-lab según bloque.
- **IA:** no permitida en la evaluación calificable ordinaria.
- **Entorno:** editor de texto/código, navegador, validador XML/XSD, herramientas XPath/XSLT, cliente HTTP/API y Git.
- **Activación:** únicamente cuando el alumno solicite expresamente presentarse.

Los ejercicios, repositorios, prácticas y simulacros pueden repetirse sin límite y no generan nota.

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
| UD01 | 8% | HTML introduce estructura semántica y base documental. |
| UD02 | 7% | CSS se evalúa como presentación y accesibilidad básica. |
| UD03 | 12% | XML es base del bloque de lenguajes estructurados. |
| UD04 | 10% | DTD/XSD exigen comprender y validar modelos de documento. |
| UD05 | 12% | XPath/XSLT introduce consulta y transformación. |
| UD06 | 14% | JSON/YAML/TOML son formatos clave para sistemas y automatización. |
| UD07 | 14% | HTTP/APIs conecta datos con servicios reales. |
| UD08 | 8% | Integración e intercambio consolidan formatos y flujos. |
| UD09 | 15% | Markdown, Git y automatización de datos se convierten en herramientas permanentes del curso. |

Total: **100% del bloque de exámenes de UD**.

## 4. Blueprint del examen final

| Bloque | UDs | Competencia | Modalidad | Dificultad | Puntos |
|---|---|---|---|---|---:|
| A. HTML/CSS | UD01-UD02 | estructurar y presentar un documento semántico y accesible | open-lab | D2-D3 | 15 |
| B. XML y validación | UD03-UD04 | construir, interpretar y validar XML | open-lab | D2-D3 | 20 |
| C. XPath/XSLT | UD05 | consultar y transformar XML | open-lab | D2-D3 | 15 |
| D. JSON/YAML/TOML | UD06 | modelar, comparar y corregir datos/configuración | open-lab | D2-D3 | 15 |
| E. HTTP/APIs e integración | UD07-UD08 | consumir/intercambiar datos y razonar sobre representación y protocolo | open-lab | D2-D4 | 20 |
| F. Markdown/Git/automatización | UD09 | documentar, versionar y producir salida reproducible | open-lab | D2-D4 | 15 |

Total: **100 puntos**.

## 5. Distribución D1-D4

| Nivel | Objetivo | Peso |
|---|---|---:|
| D1 | Comprensión | 10% |
| D2 | Aplicación | 40% |
| D3 | Diagnóstico | 30% |
| D4 | Integración / decisión | 20% |

ASIR-05 prioriza producir, validar y transformar información real. Memorizar etiquetas o sintaxis aisladas no es suficiente.

## 6. Tipos de ítem

Se podrán combinar:

- construcción/corrección de HTML;
- accesibilidad básica;
- CSS funcional;
- XML bien formado;
- namespaces;
- DTD/XSD;
- XPath;
- XSLT;
- JSON;
- YAML;
- TOML;
- comparación entre formatos;
- cabeceras HTTP;
- métodos y códigos de estado;
- consumo de API;
- interpretación de payloads;
- transformación de datos;
- Markdown;
- Git add/commit/diff/log;
- `.gitignore`;
- scripting sencillo sobre datos estructurados;
- documentación reproducible.

## 7. Modalidades

### Closed-book

Solo para fundamentos mínimos:

- diferencia estructura/presentación;
- documento bien formado vs válido;
- XML vs JSON/YAML/TOML a nivel conceptual;
- request/response HTTP;
- finalidad de Git;
- diferencia fuente de verdad/artefacto generado.

### Open-docs

Se permite documentación oficial para:

- sintaxis de XSD/XPath/XSLT;
- especificaciones de formatos;
- cabeceras/métodos HTTP;
- opciones concretas de Git;
- bibliotecas o utilidades usadas en scripting.

### Open-lab

Se permite trabajar con editor, terminal, navegador, validadores y clientes HTTP.

El objetivo es evaluar capacidad de construir y verificar datos/documentos, no memoria literal de sintaxis.

## 8. Errores críticos

Pueden invalidar un ítem práctico:

- publicar secretos o credenciales en Git;
- considerar válido un XML que no cumple el esquema requerido;
- alterar datos para forzar que una transformación “parezca correcta”;
- usar HTML sin estructura semántica cuando el requisito la exige;
- ignorar errores HTTP o códigos de estado y afirmar éxito;
- romper YAML por indentación sin detectarlo;
- sobrescribir datos fuente sin necesidad cuando se pide transformación reproducible;
- generar salida pero no poder reproducirla;
- entregar un repositorio sin historial coherente cuando el historial forma parte del objetivo.

## 9. Rúbrica de documentos y formatos

| Dimensión | Peso |
|---|---:|
| estructura correcta | 30% |
| validez / sintaxis | 25% |
| adecuación al requisito | 20% |
| verificación | 15% |
| claridad / mantenibilidad | 10% |

## 10. Rúbrica de HTTP / API

| Dimensión | Peso |
|---|---:|
| petición correcta | 20% |
| interpretación de respuesta | 25% |
| tratamiento de errores | 20% |
| representación de datos | 20% |
| verificación / explicación | 15% |

## 11. Rúbrica de Git / documentación reproducible

| Dimensión | Peso |
|---|---:|
| estructura del repositorio | 15% |
| commits coherentes | 20% |
| uso correcto de `.gitignore` | 15% |
| documentación reproducible | 25% |
| ausencia de secretos/artefactos innecesarios | 15% |
| verificación del flujo | 10% |

## 12. Exámenes de UD

### UD01

- HTML semántico;
- estructura;
- enlaces/listas/tablas/formularios básicos;
- validación.

Modalidad: open-lab.

### UD02

- CSS esencial;
- selectores;
- box model;
- layout básico;
- accesibilidad visual elemental.

Modalidad: open-lab.

### UD03

- XML bien formado;
- namespaces;
- estructura;
- errores sintácticos.

Modalidad: open-lab.

### UD04

- DTD/XSD;
- validación;
- restricciones;
- diagnóstico de documentos inválidos.

Modalidad: open-lab.

### UD05

- XPath;
- selección de nodos;
- XSLT;
- transformación;
- validación de salida.

Modalidad: open-lab.

### UD06

- JSON;
- YAML;
- TOML;
- equivalencias;
- ventajas/limitaciones;
- detección de errores.

Modalidad: open-lab.

### UD07

- HTTP;
- métodos;
- status codes;
- headers;
- payloads;
- consumo de API;
- interpretación de errores.

Modalidad: open-lab.

### UD08

- sindicación/intercambio;
- integración de fuentes;
- transformación;
- selección del formato adecuado.

Modalidad: caso aplicado.

### UD09

- Markdown;
- README;
- Git add/commit/diff/log;
- ramas intro;
- `.gitignore`;
- scripting sencillo;
- JSON/YAML;
- salida reproducible.

Modalidad: open-lab integrador.

## 13. Recuperación

La recuperación integral:

- se realiza solo cuando el alumno lo solicite;
- usa documentos/datos/APIs diferentes;
- mantiene dificultad equivalente;
- incluye validación XML;
- incluye al menos una transformación o consulta;
- incluye JSON/YAML/TOML;
- incluye un caso HTTP/API;
- incluye Git/Markdown;
- sustituye la nota de ASIR-05;
- no tiene penalización ni límite pedagógico de intentos.

## 14. Requisitos del entorno

El entorno deberá ser reproducible.

Mínimo:

- editor de texto/código;
- navegador;
- terminal;
- Git;
- repositorio local;
- validador HTML/XML/XSD;
- herramienta XPath/XSLT;
- `curl` o cliente HTTP equivalente;
- API local/de laboratorio o mock reproducible;
- Python/Bash/PowerShell introductorio cuando el ítem lo requiera;
- dataset pequeño JSON/YAML/XML.

No se dependerá de una API pública inestable para un examen calificable.

## 15. Validación del blueprint

- [x] las 9 UDs están cubiertas;
- [x] HTML/CSS están presentes sin dominar el módulo;
- [x] XML/validación tienen peso suficiente;
- [x] XPath/XSLT se evalúan de forma operativa;
- [x] JSON/YAML/TOML se evalúan como formatos profesionales;
- [x] HTTP/APIs tienen peso explícito;
- [x] Markdown/Git se consolidan como herramientas transversales;
- [x] seguridad de secretos está incluida;
- [x] D1 no domina el examen;
- [x] examen bajo demanda;
- [x] entorno reproducible.

## 16. Criterio de salida de ASIR-05

ASIR-05 se considera superado cuando el alumno puede, bajo examen:

- construir HTML semántico básico;
- aplicar CSS funcional;
- crear y validar XML;
- usar DTD/XSD;
- consultar y transformar XML con XPath/XSLT;
- trabajar con JSON, YAML y TOML;
- comprender una interacción HTTP;
- consumir e interpretar una API sencilla;
- documentar técnicamente con Markdown;
- versionar trabajo con Git;
- transformar datos de forma reproducible;
- proteger secretos y separar fuente de verdad de artefactos generados.

El objetivo es que los datos y la documentación dejen de ser “ficheros que funcionan” y pasen a ser artefactos estructurados, verificables y versionables.
