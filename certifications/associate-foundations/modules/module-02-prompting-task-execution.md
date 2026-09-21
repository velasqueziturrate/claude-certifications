# Module 02 - Prompting & Task Execution

## Learning Objectives

- Crear prompts efectivos utilizando una estructura repetible.
- Aplicar técnicas de descomposición de tareas complejas.
- Mejorar resultados mediante iteración diagnóstica.
- Adaptar la estrategia de prompting según el tipo de tarea.
- Comprender cuándo utilizar Code Execution para resultados verificables.

---

## Key Concepts

### Prompt Quality Drives Output Quality

La calidad del resultado depende principalmente de la calidad del prompt.

La diferencia entre una respuesta genérica y una respuesta útil suele deberse a la información proporcionada, no al modelo utilizado.

#### Key Takeaway

Los buenos resultados provienen de buenos prompts.

---

### Description

Description es la capacidad de comunicar exactamente lo que se necesita.

Es una competencia fundamental del AI Fluency Framework.

#### Key Takeaway

La claridad supera a la creatividad.

---

### The Five Prompt Components

Los prompts profesionales se construyen utilizando cinco componentes principales.

#### 1. Role

Quién debe ser Claude para realizar la tarea.

Ejemplos:

- Financial Analyst
- Project Manager
- Technical Architect
- Policy Reviewer

#### 2. Context

Información que Claude no puede conocer por sí mismo.

Ejemplos:

- Audiencia
- Situación
- Objetivos
- Material de referencia

#### 3. Task

La acción principal.

Ejemplos:

- Summarize
- Analyze
- Compare
- Draft
- Recommend

#### 4. Constraints

Límites y requisitos.

Ejemplos:

- Longitud
- Tono
- Exclusiones
- Reglas específicas

#### 5. Output Format

La forma del resultado.

Ejemplos:

- Tabla
- Lista
- Correo
- Memo
- Informe

---

### Context Gaps

Claude no conoce:

- Información que no ha sido proporcionada.
- Información que sólo existe en la mente del usuario.
- Información no incluida en fuentes conectadas.

#### Key Takeaway

La causa más frecuente de resultados genéricos es la falta de contexto.

---

### Prompt Diagnostics

Cuando una respuesta es deficiente, revisar los componentes del prompt.

#### Problema

Respuesta demasiado genérica.

#### Causa habitual

Falta de contexto.

---

#### Problema

Claude realiza la acción incorrecta.

#### Causa habitual

Task poco clara.

---

#### Problema

La longitud o el tono son incorrectos.

#### Causa habitual

Constraints insuficientes.

---

#### Problema

La estructura no es útil.

#### Causa habitual

Output Format no especificado.

---

### Task Decomposition

Las tareas complejas deben dividirse en pasos más pequeños.

#### Ejemplo

Malo:

Analiza estos proveedores y recomienda uno.

Mejor:

1. Extraer criterios.
2. Evaluar cada proveedor.
3. Identificar trade-offs.
4. Recomendar una opción.

#### Key Takeaway

Las tareas complejas producen mejores resultados cuando se ejecutan por etapas.

---

### Prompt Iteration

La mejora de prompts debe ser sistemática.

Proceso recomendado:

1. Revisar la respuesta.
2. Identificar el componente problemático.
3. Ajustar únicamente ese componente.
4. Volver a ejecutar.

#### Key Takeaway

Iterar sobre el componente que falla es más eficiente que reescribir todo el prompt.

---

### Task-Specific Prompting

La estrategia cambia según el objetivo.

#### Analysis

Priorizar:

- Restricciones
- Criterios
- Evidencia

---

#### Research

Priorizar:

- Profundidad
- Cobertura
- Fuentes

---

#### Drafting

Priorizar:

- Audiencia
- Tono
- Formato

---

#### Brainstorming

Priorizar:

- Diversidad
- Cantidad
- Creatividad

Reducir restricciones al inicio.

---

### Verified Computation

Cuando existen cálculos importantes, debe utilizarse Code Execution.

#### Examples

- Medias
- Proyecciones
- Cálculos financieros
- Procesamiento de datos

#### Key Takeaway

Code Execution produce resultados calculados y verificables, no estimaciones plausibles.

---

## Summary

### Main Ideas

- La estructura del prompt determina la calidad del resultado.
- Los cinco componentes cubren prácticamente todos los casos profesionales.
- El contexto es el componente más olvidado.
- Las tareas complejas deben dividirse.
- La iteración debe ser diagnóstica.
- Las estrategias cambian según el tipo de trabajo.
- Los cálculos importantes requieren Code Execution.

### Important Details

- Role define la perspectiva.
- Context aporta conocimiento situacional.
- Task define la acción.
- Constraints limitan la respuesta.
- Output Format define la estructura.

### Best Practices

- Utilizar explícitamente los cinco componentes.
- Proporcionar contexto suficiente.
- Dividir trabajos complejos.
- Ajustar únicamente el componente problemático.
- Usar Code Execution para cálculos.

---

## Personal Notes

### Regla de oro

Role → Context → Task → Constraints → Output Format

### Probables preguntas de examen

- Componentes de un prompt.
- Context gaps.
- Task decomposition.
- Prompt diagnostics.
- Brainstorming vs Analysis.
- Code Execution.

---

## Potential Exam Questions

### Question 1

¿Cuál es la competencia principal del AI Fluency Framework cubierta en este módulo?

**Answer:**

Description.

---

### Question 2

¿Cuáles son los cinco componentes de un prompt efectivo?

**Answer:**

Role, Context, Task, Constraints y Output Format.

---

### Question 3

¿Qué componente define quién debe ser Claude durante una tarea?

**Answer:**

Role.

---

### Question 4

¿Qué componente suele omitirse con mayor frecuencia por los usuarios?

**Answer:**

Context.

---

### Question 5

¿Qué suele ocurrir cuando falta contexto?

**Answer:**

Las respuestas se vuelven genéricas o poco relevantes.

---

### Question 6

¿Qué componente define la acción principal que debe realizar Claude?

**Answer:**

Task.

---

### Question 7

¿Qué componente controla longitud, tono y restricciones?

**Answer:**

Constraints.

---

### Question 8

¿Por qué es recomendable especificar el Output Format?

**Answer:**

Porque reduce iteraciones y mejora la utilidad inmediata del resultado.

---

### Question 9

¿Qué es un Context Gap?

**Answer:**

Información que Claude necesita para realizar la tarea pero que no ha sido proporcionada explícitamente.

---

### Question 10

¿Cuál es la mejor forma de diagnosticar un prompt débil?

**Answer:**

Revisar los cinco componentes del Prompt Stack.

---

### Question 11

¿Qué problema suele indicar un Task ambiguo?

**Answer:**

Claude responde a una pregunta diferente de la que realmente se quería plantear.

---

### Question 12

¿Qué es Task Decomposition?

**Answer:**

Dividir una tarea compleja en pasos más pequeños y secuenciales.

---

### Question 13

¿Cuál es una ventaja principal de Task Decomposition?

**Answer:**

Permite validar resultados intermedios antes de llegar al resultado final.

---

### Question 14

¿Cuándo conviene mantener varios pasos en la misma conversación?

**Answer:**

Cuando cada paso depende de los resultados generados en pasos anteriores.

---

### Question 15

¿Cuándo conviene abrir una conversación nueva?

**Answer:**

Cuando la tarea es independiente o el contexto se ha degradado.

---

### Question 16

¿Cómo debe realizarse la iteración de prompts?

**Answer:**

Identificando el componente que falla y modificando únicamente ese componente.

---

### Question 17

¿Cuándo debe detenerse el proceso de iteración?

**Answer:**

Cuando los cambios son marginales y el beneficio adicional es mínimo.

---

### Question 18

¿Qué tipo de tareas requieren más restricciones y criterios explícitos?

**Answer:**

Las tareas de análisis (Analysis).

---

### Question 19

¿Qué tipo de tarea requiere mayor libertad creativa y menos restricciones?

**Answer:**

Brainstorming.

---

### Question 20

¿En qué orden se recomienda construir un prompt complejo?

**Answer:**

Role → Context → Task → Constraints → Output Format.
---

## Flashcards

Q: ¿Qué componente suelen olvidar más los usuarios?

A: Context.

---

Q: ¿Qué componente define la acción principal?

A: Task.

---

Q: ¿Qué componente define el formato de salida?

A: Output Format.

---

Q: ¿Qué técnica mejora tareas complejas?

A: Task Decomposition.

---

Q: ¿Cómo debe mejorarse un prompt?

A: Identificando y corrigiendo el componente problemático.

---

Q: ¿Qué necesita brainstorming?

A: Más libertad y menos restricciones iniciales.

---

Q: ¿Cuándo usar Code Execution?

A: Cuando la precisión numérica importa.

---

## References

- Associate Foundations Training Material
- Anthropic Prompting Guidance

---

## Review Status

- [x] Reviewed once
- [ ] Reviewed twice
- [ ] Included in final cheatsheet