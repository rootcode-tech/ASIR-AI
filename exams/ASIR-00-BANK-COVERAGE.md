# ASIR-00 · Cobertura requerida del banco calificable

**Versión:** 0.1.0  
**Estado:** pendiente de completar antes del examen final  
**No bloquea:** enseñanza, ejercicios, laboratorios ni simulacros formativos

## 1. Motivo

El banco v0.1 tiene cobertura mínima por UD, pero la arquitectura de evaluación exige poder construir:
- un examen ordinario;
- una recuperación equivalente;
- sin reutilizar una única pregunta crítica;
- sin generación de ítems calificables por LLM en tiempo de examen.

La nueva prueba por dominios necesita cobertura mucho más granular.

## 2. Objetivo mínimo recomendado

| Dominio | Forma oficial de referencia | Objetivo de banco |
|---|---|---:|
| EO | entrevista + imagen | 6 paquetes orales |
| CO | 5 preguntas/audio | 4 audios × 5 ítems |
| EE | 1 desarrollo | 6 prompts |
| CE | 8 test | 20 ítems |
| NC | 8 test | 20 ítems |
| FM | 8 test | 20 ítems |
| GE | 8 test | 20 ítems |
| IAD | 8 test | 20 ítems |
| CC | 8 test | 20 ítems |
| CCD | 8 test | 20 ítems |
| SEG | 8 test | 20 ítems |
| PRO | 8 test | 20 ítems |
| Inglés | 16 test | 40 ítems |
| Tecnología e Ingeniería | 16 test | 40 ítems |

El objetivo incorpora margen sobre el mínimo matemático para ordinario + recuperación.

## 3. Cobertura cualitativa obligatoria

### GE
Debe incluir:
- varianza/desviación;
- tablas de contingencia;
- covarianza;
- correlación;
- regresión;
- condicional;
- independencia;
- total;
- Bayes;
- tasas base.

### Digital
Debe existir cobertura separada de:
- IAD;
- CC;
- CCD;
- SEG;
- PRO.

### Inglés
Debe mezclar:
- reading;
- uso funcional;
- registro;
- tiempos verbales;
- comparación/opinión;
- reformulación/mediación;
- instrucciones y contexto profesional.

### Tecnología e Ingeniería
Debe cubrir TI4.1–TI4.5:
- proyectos/mecánica/materiales;
- electricidad/electrónica/automática;
- térmica/neumática;
- geometría/transformaciones;
- representación/normalización.

## 4. Reglas editoriales

Todo ítem calificable:
- se redacta antes del examen;
- se revisa;
- recibe solución/rúbrica;
- se marca `approved`;
- declara dominio;
- declara dificultad;
- no copia literalmente preguntas oficiales;
- tiene distractores derivados de errores plausibles;
- no depende de información externa inestable.

## 5. Gate técnico

```text
teaching_ready = true
final_exam_ready = false
```

hasta que:
1. se alcancen los mínimos;
2. se valide el esquema;
3. se generen al menos dos formas equivalentes;
4. se compruebe duración;
5. se haga revisión editorial final.

## 6. Momento de completarlo

No es necesario terminar este volumen antes de empezar UD01.

Debe completarse **antes de entrar en la fase de examen calificable**, idealmente durante/antes de los simulacros finales, para que los ítems no condicionen la enseñanza inicial.
