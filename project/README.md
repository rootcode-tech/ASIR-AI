# Proyecto ASIR-AI

Proyecto integrador continuo que evolucionará desde primer curso y culminará en una infraestructura profesional reproducible y documentada.

## Dirección de producto propuesta

Además de ser el proyecto académico final, ASIR-AI podrá convertirse en el prototipo de una plataforma educativa comercial.

Concepto:

**una web para aprender ASIR desde cero, con tutoría IA, laboratorios guiados y un profesor virtual que explique cada lección en vídeo.**

## Experiencia de usuario

La plataforma podría ofrecer:

```text
asignatura
   ↓
UD
   ↓
lección explicada
   ↓
vídeo del profesor virtual
   ↓
texto / diagramas / ejemplos
   ↓
preguntas al tutor IA
   ↓
ejercicios
   ↓
laboratorio guiado
   ↓
simulacro
   ↓
examen solo cuando el alumno quiera presentarse
```

## Profesor virtual con IA

Cada lección podría disponer de un vídeo generado a partir del contenido aprobado de la UD.

Formato inicial:

- avatar sintético o personaje propio;
- encuadre tipo webcam/profesor;
- voz sintética licenciada o propia;
- explicación sincronizada con diagramas, terminal, slides o demostraciones;
- transcripción accesible;
- controles de velocidad y subtítulos;
- enlaces desde el vídeo al punto exacto de la documentación.

La fuente de verdad seguirá siendo el contenido versionado del curso. El vídeo será una representación derivada, no una fuente independiente.

## Tutor IA

El tutor de la plataforma deberá poder:

- explicar el mismo concepto de distintas formas;
- responder preguntas sobre la lección;
- detectar prerequisitos no comprendidos;
- generar ejemplos adicionales;
- proponer ejercicios;
- revisar respuestas;
- guiar troubleshooting sin regalar la solución demasiado pronto;
- preparar simulacros;
- respetar que el examen solo comienza por decisión expresa del alumno.

## Arquitectura conceptual del producto

Posible evolución:

- frontend web;
- autenticación;
- perfiles y progreso;
- motor de contenidos Markdown/YAML;
- API;
- base de datos;
- reproductor de vídeo;
- generación/almacenamiento de vídeos;
- tutor IA con retrieval sobre contenidos del curso;
- sistema de ejercicios;
- laboratorios;
- sistema de exámenes;
- analítica de progreso;
- panel de autor;
- versionado de contenido;
- pagos/suscripciones solo si se valida comercialmente.

## Principio de contenido

```text
Markdown/YAML versionado
        ↓
contenido aprobado
        ↓
web
   ↙          ↘
vídeo IA     tutor IA
```

Esto evita que el avatar o el modelo inventen el currículo por separado.

## Valor comercial potencial

El producto sería diferencial si demuestra:

- explicación realmente comprensible desde cero;
- tutoría ilimitada;
- progresión personalizada;
- laboratorios reproducibles;
- exámenes voluntarios bajo demanda;
- currículo técnico serio;
- contenido verificable y versionado;
- preparación profesional y portfolio.

La comercialización solo se planteará después de demostrar que el sistema enseña de forma efectiva mediante uso real, feedback y métricas.

## Consideraciones de producto

Antes de venderlo habrá que resolver, entre otras:

- derechos/licencias de contenido;
- licencias de voz/avatar;
- privacidad;
- protección de datos;
- accesibilidad;
- costes de inferencia y generación de vídeo;
- actualización de tecnologías;
- control de calidad de respuestas IA;
- prevención de alucinaciones;
- seguridad de laboratorios;
- términos de uso;
- modelo comercial.

## Relación con ASIR-17

El proyecto final podrá utilizar esta propia plataforma como producto demostrador.

La infraestructura técnica del proyecto deberá seguir cumpliendo los requisitos de ASIR-17: red, sistemas, identidad, datos, servicios, seguridad, automatización, CI/CD, observabilidad, backup, recuperación, documentación y defensa.

Así, el proyecto no sería solo “hacer una web”, sino construir y operar la plataforma completa que imparte ASIR-AI.
