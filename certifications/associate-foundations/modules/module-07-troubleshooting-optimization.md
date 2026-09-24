# Module 07 - Troubleshooting & Optimization

## Learning Objectives

- Diagnosticar por qué un prompt o una respuesta están funcionando mal.
- Identificar la causa raíz entre especificación, contexto, configuración y selección de herramientas.
- Convertir feedback en mejoras persistentes.
- Optimizar workflows eliminando fricción y redundancia.
- Promover correcciones recurrentes a configuración reutilizable.
- Medir mejoras de eficiencia y consistencia.

---

## Key Concepts

### Underperformance Has Discoverable Causes

Cuando Claude produce un mal resultado, normalmente ocurre una de estas dos cosas:

- El usuario abandona y concluye que Claude no puede hacerlo.
- El usuario cambia cosas aleatoriamente hasta que algo funciona.

El enfoque correcto es el diagnóstico estructurado.

### Key Takeaway

La mayoría de problemas tienen una causa identificable y una solución concreta.

---

## Four Common Failure Patterns

### 1. Under-Specification

Síntoma:

> La primera respuesta ya es incorrecta.

Causa:

Falta información importante en el prompt.

Ejemplos:

- Contexto insuficiente.
- Restricciones ausentes.
- Formato no definido.

### Fix

Añadir:

- Context
- Constraints
- Output Format

---

### 2. Context Overload

Síntoma:

> La conversación empezó bien y se degradó con el tiempo.

Causa:

El contexto se ha vuelto demasiado largo.

Las instrucciones iniciales se han resumido o perdido importancia.

### Fix

- Restart
- Summarize
- Persist

### Exam Connection

Relacionado directamente con el Módulo 1.

---

### 3. Wrong Feature or Model

Síntoma:

> Error específico y repetible.

Ejemplos:

- Cálculos incorrectos.
- Análisis superficiales.
- Resultados limitados.

### Typical Causes

- No usar Code Execution.
- Modelo demasiado ligero.
- Herramienta equivocada.

### Fix

Seleccionar la funcionalidad adecuada.

---

### 4. Stale Configuration

Síntoma:

> Antes funcionaba correctamente.

Causa:

- Instructions obsoletas.
- Knowledge Base desactualizada.
- Skills antiguas.
- Memory degradada.

### Fix

Aplicar mantenimiento de configuración.

### Exam Connection

Relacionado directamente con el Módulo 5.

---

## Diagnostic Sequence

Antes de concluir que Claude no puede realizar una tarea:

### Step 1

Revisar especificación.

Pregunta:

> ¿Está correctamente definido el prompt?

---

### Step 2

Revisar contexto.

Pregunta:

> ¿Existe sobrecarga de contexto?

---

### Step 3

Revisar modelo y herramientas.

Preguntas:

- ¿Necesita Code Execution?
- ¿Necesita un modelo más potente?

---

### Step 4

Revisar configuración.

Preguntas:

- ¿Instructions actualizadas?
- ¿Knowledge correcta?
- ¿Skills vigentes?

---

### Step 5

Evaluar si el problema es adecuado para Claude.

Pregunta:

> ¿Existe una incompatibilidad fundamental entre el problema y la herramienta?

---

## Cheapest Fix First Principle

La secuencia sigue el orden de menor coste.

### Cheapest

Corregir el prompt.

---

### Medium Cost

Restart o cambio de configuración.

---

### Higher Cost

Cambiar modelo o herramientas.

---

### Highest Cost

Reformular completamente la tarea.

### Key Takeaway

No empezar por la solución más costosa.

---

## Expectation Mismatch

Algunos problemas no tienen solución mediante prompts.

### Example

> Predict next quarter's exact sales.

Problema:

Claude no puede predecir el futuro con precisión.

### Better Approach

Pedir:

- Escenarios.
- Rangos.
- Hipótesis.
- Factores explicativos.

### Key Takeaway

Algunas tareas requieren replantear la pregunta.

---

## Feedback as Diagnostic Data

Cada resultado decepcionante contiene información útil.

### Wrong Approach

Corregir manualmente cada vez.

---

### Correct Approach

Identificar:

- Qué problema existe.
- Qué lo provoca.
- Cómo evitarlo en el futuro.

---

## From Reaction to Instruction

### Reaction

> Too generic

---

### Better Instruction

> Add audience and desired action.

---

### Reaction

> Missed the point

---

### Better Instruction

> Explicitly state the primary question the output must answer.

### Key Takeaway

Transformar opiniones subjetivas en instrucciones concretas.

---

## Capture What Works

Cuando una solución funciona:

No dejarla en una conversación.

Promoverla.

---

### Promotion Targets

#### Standing Instructions

Reglas.

---

#### Skills

Procedimientos.

---

#### Knowledge Base

Material de referencia.

### Key Takeaway

Una corrección recurrente debe convertirse en configuración.

---

## Capture vs Lose

### Captured Fix

Corrección convertida en configuración.

Beneficio:

Desaparece el problema para todos.

---

### Lost Fix

Corrección repetida manualmente en cada ejecución.

Coste:

El problema reaparece indefinidamente.

---

## Workflow Optimization

La optimización debe realizarse deliberadamente.

---

## Find Friction

Tres señales indican oportunidades de mejora.

---

### Repetition

Síntoma:

Repetir exactamente la misma información.

### Fix

Standing Instructions o contexto persistente.

---

### Correction

Síntoma:

Corregir siempre el mismo error.

### Fix

Modificar configuración.

---

### Variance

Síntoma:

Distintos usuarios producen resultados distintos.

### Fix

Skills compartidas y Knowledge Base común.

---

## Consolidate & Promote

Dos acciones generan la mayor parte de las mejoras.

### Consolidate

Combinar pasos separados cuando sea posible.

---

### Promote

Convertir patrones repetitivos en configuración.

---

## Rule / Reference / Procedure Test

### Rule

Comportamiento.

Destino:

Standing Instructions.

---

### Reference

Información.

Destino:

Knowledge Base.

---

### Procedure

Secuencia de pasos.

Destino:

Skills.

### Exam Note

Tema muy probable de examen por su conexión con el Módulo 5.

---

## Validate Optimizations

No todo cambio mejora el workflow.

### Recommendation

Probar varias ejecuciones antes de institucionalizar una optimización.

### Risk

Un error promovido a configuración afecta a todos los usuarios.

---

## Measure Improvement

La optimización debe poder medirse.

### Possible Metrics

#### Time Saved

Tiempo reducido.

---

#### Consistency

Menor variabilidad.

---

#### Quality

Menos errores.

---

#### Revision Rounds

Menos iteraciones.

### Key Takeaway

Lo que no puede medirse es difícil de justificar.

---

## Workflow Audit Example

### Before

- 45 minutos por analista.
- Formatos inconsistentes.
- Correcciones repetidas.

---

### Changes

#### Knowledge Base

Contexto compartido.

#### Skill

Formato común.

#### Standing Instruction

Verificación estandarizada.

---

### After

- 25 minutos por analista.
- Formato consistente.
- Menos revisiones.

### Key Takeaway

La optimización genera beneficios acumulativos.

---

## Key Takeaways

### 1. Underperformance Has Discoverable Causes

Aplicar la secuencia diagnóstica antes de culpar a la herramienta.

---

### 2. Isolate Before You Fix

Identificar si el problema es:

- Prompt
- Context
- Feature
- Configuration
- Expectation Mismatch

---

### 3. Every Bad Output Is Data

Convertir feedback en ajustes concretos.

---

### 4. Optimize Deliberately

Identificar fricción, promover correcciones y medir resultados.

---

## Summary

### Main Ideas

- Los problemas tienen causas identificables.
- La secuencia diagnóstica evita soluciones aleatorias.
- Algunas tareas requieren herramientas distintas.
- El feedback debe convertirse en mejoras persistentes.
- La optimización se basa en eliminar fricción.
- Las correcciones recurrentes deben convertirse en configuración.
- La mejora debe medirse.

### Important Details

- Under-Specification
- Context Overload
- Wrong Feature or Model
- Stale Configuration
- Diagnostic Sequence
- Expectation Mismatch
- Promotion
- Rule / Reference / Procedure
- Optimization Metrics

### Best Practices

- Aplicar la secuencia completa antes de cambiar de modelo.
- Capturar correcciones exitosas.
- Promover reglas, referencias y procedimientos al lugar correcto.
- Probar optimizaciones antes de institucionalizarlas.
- Medir siempre la mejora conseguida.

---

## Personal Notes

### Fórmulas de examen

Diagnóstico:

Under-Specification →
Context →
Feature →
Configuration →
Task Fit

Promoción:

Rule → Instructions

Reference → Knowledge

Procedure → Skills

Optimización:

Repetition →
Correction →
Variance

---

## Exam Hot Topics

- Under-Specification
- Context Overload
- Wrong Feature
- Wrong Model
- Stale Configuration
- Diagnostic Sequence
- Expectation Mismatch
- Feedback Loops
- Capture vs Promote
- Workflow Friction
- Rule / Reference / Procedure
- Workflow Audits
- Optimization Metrics

---

## Potential Exam Questions

### Question 1

¿Cuáles son los cuatro patrones principales de fallo?

**Answer:** Under-Specification, Context Overload, Wrong Feature/Model y Stale Configuration.

---

### Question 2

¿Qué indica que la primera respuesta ya sea incorrecta?

**Answer:** Under-Specification.

---

### Question 3

¿Qué indica que el rendimiento se degrade con el tiempo?

**Answer:** Context Overload.

---

### Question 4

¿Qué suele solucionar errores numéricos repetidos?

**Answer:** Code Execution.

---

### Question 5

¿Qué indica la frase “antes funcionaba”?

**Answer:** Stale Configuration.

---

### Question 6

¿Cuál es el primer paso del proceso diagnóstico?

**Answer:** Revisar la especificación del prompt.

---

### Question 7

¿Cuál es el último paso del proceso diagnóstico?

**Answer:** Evaluar si la tarea es adecuada para Claude.

---

### Question 8

¿Qué es un Expectation Mismatch?

**Answer:** Un problema que no puede resolverse simplemente mejorando el prompt.

---

### Question 9

¿Qué debe hacerse con una corrección recurrente?

**Answer:** Capturarla en configuración.

---

### Question 10

¿Qué diferencia existe entre reacción e instrucción?

**Answer:** La reacción expresa una opinión; la instrucción identifica un cambio concreto.

---

### Question 11

¿Qué significa Promotion?

**Answer:** Convertir soluciones recurrentes en configuración reutilizable.

---

### Question 12

¿Dónde deberían almacenarse las reglas?

**Answer:** Standing Instructions.

---

### Question 13

¿Dónde deberían almacenarse las referencias?

**Answer:** Knowledge Base.

---

### Question 14

¿Dónde deberían almacenarse los procedimientos?

**Answer:** Skills.

---

### Question 15

¿Qué indica Repetition?

**Answer:** Información repetida manualmente.

---

### Question 16

¿Qué indica Correction?

**Answer:** El mismo error corregido repetidamente.

---

### Question 17

¿Qué indica Variance?

**Answer:** Resultados diferentes para el mismo trabajo.

---

### Question 18

¿Qué es Consolidation?

**Answer:** Agrupar pasos que pueden ejecutarse conjuntamente.

---

### Question 19

¿Qué debe hacerse antes de desplegar una optimización?

**Answer:** Validarla en varias ejecuciones.

---

### Question 20

¿Cuál es la idea principal del módulo?

**Answer:** Diagnosticar sistemáticamente y convertir mejoras en resultados persistentes.

---

## Flashcards

Q: ¿Qué patrón aparece cuando la primera respuesta ya es incorrecta?

A: Under-Specification.

---

Q: ¿Qué patrón aparece cuando una conversación se degrada?

A: Context Overload.

---

Q: ¿Qué suele solucionar errores numéricos?

A: Code Execution.

---

Q: ¿Qué es Stale Configuration?

A: Configuración que antes funcionaba y ahora está obsoleta.

---

Q: ¿Qué es Expectation Mismatch?

A: Una tarea que necesita replantearse.

---

Q: ¿Qué es Promotion?

A: Convertir una corrección en configuración reutilizable.

---

Q: ¿Dónde van las reglas?

A: Standing Instructions.

---

Q: ¿Dónde van las referencias?

A: Knowledge Base.

---

Q: ¿Dónde van los procedimientos?

A: Skills.

---

Q: ¿Cuál es la regla principal del módulo?

A: Diagnosticar primero, optimizar después.

---

## Review Status

- [x] Reviewed once
- [ ] Reviewed twice
- [ ] Included in final cheatsheet