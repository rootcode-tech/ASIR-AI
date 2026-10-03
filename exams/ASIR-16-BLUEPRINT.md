# ASIR-16 · Especialización — DevOps, Cloud e IA para Sistemas

## Blueprint de evaluación

Este documento define la arquitectura de evaluación de **ASIR-16 · Especialización — DevOps, Cloud e IA para Sistemas**.

El módulo integra Git profesional, automatización, contenedores, CI/CD, Ansible, Terraform, cloud, Kubernetes, observabilidad, SRE e IA aplicada a sistemas. La evaluación debe comprobar que el alumno puede construir, automatizar, desplegar, observar y recuperar una infraestructura reproducible, no simplemente ejecutar comandos aislados.

El examen solo comienza cuando el alumno lo solicita de forma explícita.

## 1. Perfil del examen

- **Tipo:** examen técnico práctico e integrador.
- **Duración orientativa:** 180-210 minutos.
- **Modalidad:** open-docs + open-lab en la mayor parte del examen.
- **IA:** no permitida en los bloques ordinarios; permitida de forma controlada únicamente en los ejercicios diseñados para evaluar uso profesional de IA.
- **Entorno:** laboratorio aislado y reproducible con Linux, Git, Docker/Compose, pipeline CI/CD, Ansible, Terraform, recursos cloud simulados o reales controlados, Kubernetes introductorio y stack de observabilidad.
- **Principio:** la competencia se demuestra mediante configuración, ejecución, evidencia, verificación y recuperación.

## 2. Cálculo de la calificación

Se aplica el marco general del proyecto:

- **60 %**: exámenes de UD ponderados.
- **40 %**: examen final integrador.
- Nota mínima del examen final: **5,0 / 10**.
- Nota final mínima de la asignatura: **5,0 / 10**.

Los ejercicios, laboratorios, repositorios y proyectos previos son formativos y no aportan puntuación directa a la nota.

## 3. Peso de los exámenes por UD

| UD | Contenido | Peso dentro del 60 % |
|---|---|---:|
| UD01 | Flujo profesional con Git, ramas, PR, releases y SemVer | 10 % |
| UD02 | Linux para DevOps y automatización reproducible | 8 % |
| UD03 | Docker: imágenes, contenedores, redes y volúmenes | 10 % |
| UD04 | Docker Compose y stacks multi-servicio | 10 % |
| UD05 | CI/CD con pipelines y quality gates | 12 % |
| UD06 | Ansible: inventarios, playbooks, roles e idempotencia | 12 % |
| UD07 | Terraform e Infrastructure as Code | 12 % |
| UD08 | Cloud: IAM, redes, compute, storage y costes | 10 % |
| UD09 | Kubernetes: arquitectura y operación introductoria | 7 % |
| UD10 | Observabilidad, SRE, IA asistida y proyecto DevOps | 9 % |
|  | **Total** | **100 %** |

## 4. Blueprint del examen final integrador

| Bloque | Competencia principal | UDs | Puntos |
|---|---|---|---:|
| Git y flujo de entrega | gestionar cambios, ramas, integración, releases y trazabilidad | UD01 | 10 |
| Contenedores y Compose | construir y operar un stack reproducible y persistente | UD03-UD04 | 20 |
| CI/CD | diseñar un pipeline verificable con quality gates y despliegue controlado | UD05 | 15 |
| Ansible | automatizar configuración de forma idempotente | UD06 | 15 |
| Terraform + cloud | definir infraestructura declarativa, segura y reproducible | UD07-UD08 | 20 |
| Kubernetes | interpretar y operar un despliegue introductorio | UD09 | 10 |
| Observabilidad / SRE / IA | diagnosticar un incidente con métricas, logs, alertas y uso crítico de IA | UD10 | 10 |
|  | **Total** |  | **100** |

## 5. Distribución de dificultad

ASIR-16 debe concentrarse en análisis e integración:

- **D1 · Reconocimiento / comprensión:** 5 %
- **D2 · Aplicación:** 25 %
- **D3 · Diagnóstico / análisis:** 35 %
- **D4 · Integración / decisión:** 35 %

El examen no debe premiar la memorización de sintaxis que puede consultarse en documentación oficial.

## 6. Tipos de ítems

Se podrán utilizar:

- interpretación de `git log`, `diff`, ramas y conflictos;
- corrección de un flujo de Git defectuoso;
- creación o revisión de `Dockerfile`;
- construcción y ejecución de imágenes;
- diagnóstico de redes, volúmenes y persistencia Docker;
- diseño y corrección de `compose.yml`;
- pipelines con build, test, lint, análisis y deploy;
- lectura de logs de pipeline;
- inventarios, playbooks, handlers y roles de Ansible;
- comprobación de idempotencia;
- `terraform plan`, estado, variables, outputs y dependencias;
- IAM y mínimo privilegio;
- arquitectura cloud básica con red, compute y storage;
- estimación razonada de costes;
- manifiestos Kubernetes sencillos;
- diagnóstico de Pod, Deployment, Service, ConfigMap y Secret;
- métricas, logs, alertas y SLI/SLO introductorios;
- análisis de un incidente con evidencias;
- bloque controlado de IA con validación explícita de la respuesta producida.

## 7. Regla transversal de automatización

Toda automatización relevante debe respetar esta secuencia:

```text
comprender el componente
        ↓
hacerlo manualmente
        ↓
verificarlo
        ↓
documentar el procedimiento
        ↓
automatizar
        ↓
repetir la ejecución
        ↓
comprobar idempotencia
        ↓
observar y mantener
```

Un recurso automatizado que solo funciona en la primera ejecución no demuestra competencia suficiente.

## 8. Errores críticos

Podrán penalizar severamente o invalidar el bloque afectado:

- subir secretos, claves o tokens reales al repositorio;
- incluir contraseñas en texto plano en código, imágenes o pipelines sin necesidad justificada;
- ejecutar `terraform apply` destructivo sin comprender el plan;
- perder o manipular el estado de Terraform de forma insegura;
- usar permisos IAM excesivos para resolver un problema;
- usar imágenes con tag mutable como única garantía de reproducibilidad en un ejercicio que exige versionado;
- confundir almacenamiento efímero con persistencia;
- destruir volúmenes sin haber identificado el impacto;
- considerar idempotente una automatización que modifica el sistema en cada ejecución;
- saltarse tests o quality gates para forzar un deploy;
- desactivar controles de seguridad para “hacer que funcione”;
- afirmar que un servicio está sano sin health check o verificación equivalente;
- modificar producción simulada sin estrategia de rollback cuando el caso la exige;
- copiar una respuesta de IA y aplicarla sin validación;
- introducir código o configuración sugeridos por IA que expongan secretos o rompan seguridad;
- declarar solucionado un incidente sin evidencia posterior al cambio.

## 9. Rúbrica de automatización e Infrastructure as Code

| Criterio | Peso |
|---|---:|
| Resultado funcional correcto | 25 % |
| Reproducibilidad | 20 % |
| Idempotencia / convergencia | 15 % |
| Seguridad y gestión de secretos | 15 % |
| Verificación y evidencias | 15 % |
| Claridad y mantenibilidad | 10 % |

## 10. Rúbrica de CI/CD

| Criterio | Peso |
|---|---:|
| Pipeline válido y ejecutable | 20 % |
| Build y tests | 20 % |
| Quality gates | 15 % |
| Gestión correcta de artefactos / versiones | 15 % |
| Secretos y permisos | 15 % |
| Deploy, verificación y rollback | 15 % |

## 11. Rúbrica de troubleshooting DevOps

| Criterio | Peso |
|---|---:|
| Delimitación del síntoma | 10 % |
| Recogida de evidencias | 20 % |
| Hipótesis razonadas | 20 % |
| Prueba controlada | 15 % |
| Corrección mínima y segura | 15 % |
| Validación posterior | 10 % |
| RCA / documentación | 10 % |

## 12. Bloque de IA controlada

La IA solo se utilizará cuando la competencia evaluada sea precisamente su uso profesional.

El alumno puede recibir una respuesta de un modelo o solicitar una propuesta dentro de un entorno controlado. Debe ser capaz de:

1. identificar qué afirma la IA;
2. detectar suposiciones o posibles errores;
3. contrastar con documentación, estado real del sistema o pruebas;
4. corregir la propuesta si procede;
5. ejecutar de forma segura;
6. verificar el resultado;
7. explicar qué parte de la respuesta era útil, incorrecta o incompleta.

La respuesta de la IA nunca se considera evidencia suficiente por sí sola.

## 13. Entorno reproducible de examen

El laboratorio debería poder reconstruirse automáticamente e incluir, cuando proceda:

- repositorio Git preparado con ramas, commits y conflictos controlados;
- runner CI/CD aislado;
- aplicación pequeña con tests;
- registry local o equivalente;
- Docker Engine y Docker Compose;
- varias máquinas o contenedores para Ansible;
- backend/state de Terraform seguro y desechable;
- proveedor cloud simulado, sandbox o cuenta educativa limitada;
- clúster Kubernetes local tipo `kind`, `k3d`, `minikube` o equivalente;
- Prometheus/Grafana/Loki o stack equivalente cuando el bloque lo requiera;
- fallos inyectados y reproducibles;
- scripts de reset;
- datasets/configuraciones sin datos personales ni secretos reales.

## 14. Corrección determinista

Siempre que sea posible, la plataforma podrá comprobar automáticamente:

- estado y ramas Git esperadas;
- existencia de tags o versiones;
- build correcto de imágenes;
- health checks;
- persistencia de datos;
- conectividad entre servicios;
- salida de tests;
- resultado de pipelines;
- segunda ejecución de Ansible sin cambios inesperados;
- `terraform validate` y propiedades concretas del plan;
- recursos previstos en el estado;
- políticas IAM esperadas;
- estado de Pods, Deployments y Services;
- presencia de métricas o logs esperados;
- recuperación del servicio tras una incidencia.

La corrección automática no sustituye la valoración del razonamiento, seguridad y justificación técnica.

## 15. Recuperación

La recuperación utilizará otro escenario, repositorio, stack, proveedor simulado e incidente, pero mantendrá las mismas competencias y nivel de dificultad.

No existe penalización por intentos previos ni techo de nota.

El alumno decide cuándo está preparado para solicitarla.

## 16. Criterio de dominio de salida

Para superar ASIR-16 el alumno debe poder demostrar que sabe:

- trabajar con Git usando ramas, revisiones y releases coherentes;
- construir imágenes Docker reproducibles y razonablemente seguras;
- desplegar stacks multi-servicio con persistencia y redes correctas;
- diseñar un pipeline CI/CD con controles de calidad;
- automatizar configuración con Ansible de forma idempotente;
- describir infraestructura con Terraform y comprender `plan`, `apply`, state y drift;
- aplicar mínimo privilegio en cloud;
- interpretar costes y dependencias básicas de una arquitectura cloud;
- desplegar y diagnosticar recursos Kubernetes introductorios;
- observar sistemas mediante métricas, logs y alertas;
- razonar con principios básicos de SRE;
- utilizar IA como asistente técnico sin delegar la validación;
- explicar, verificar, revertir y documentar sus decisiones.

## 17. Principio pedagógico del módulo

```text
manual
  ↓
reproducible
  ↓
automatizado
  ↓
versionado
  ↓
validado
  ↓
observable
  ↓
recuperable
```

El objetivo de ASIR-16 no es aprender una colección de herramientas DevOps. Es aprender a operar infraestructura moderna de forma declarativa, repetible, segura, verificable y mantenible.
