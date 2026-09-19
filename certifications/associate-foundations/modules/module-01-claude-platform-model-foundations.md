# Module 01 - Claude Platform & Model Foundations

## Learning Objectives

- Comprender el funcionamiento básico de la IA generativa y Claude.
- Diferenciar los distintos puntos de entrada de Claude (Chat, Projects, Artifacts y Research).
- Entender las limitaciones de contexto y memoria.
- Seleccionar la configuración adecuada para distintos escenarios profesionales.
- Comprender los trade-offs entre modelos y capacidades.

---

## Key Concepts

### Responses Vary

Claude genera respuestas probabilísticamente.

La misma pregunta puede producir respuestas distintas en diferentes ejecuciones.

#### Key Takeaway

La variabilidad es una característica normal de la IA generativa.

---

### Confidence ≠ Accuracy

Un tono seguro no garantiza que la información sea correcta.

Las respuestas incorrectas pueden parecer completamente fiables.

#### Key Takeaway

Siempre verificar información importante.

---

### Context Is a Budget

Las conversaciones tienen una capacidad limitada de contexto.

A medida que una conversación crece:

- El contexto se consume.
- Parte del historial puede resumirse.
- Instrucciones antiguas pueden perder influencia.

#### Key Takeaway

El contexto es un recurso finito.

---

### Training Boundary

Claude tiene una fecha límite de entrenamiento.

Para información actual es necesario utilizar:

- Web Search
- Research
- Fuentes externas

#### Key Takeaway

El modelo no conoce automáticamente información posterior a su entrenamiento.

---

### Configured Processes Still Vary

Incluso con prompts e instrucciones bien definidas pueden existir diferencias entre respuestas.

#### Key Takeaway

Los procedimientos reducen la variabilidad, pero no la eliminan.

---

### Chat

Conversación estándar.

#### Best Use Cases

- Preguntas rápidas
- Borradores
- Exploración
- Tareas puntuales

#### Limitation

No mantiene contexto estructurado entre sesiones.

---

### Projects

Espacios de trabajo persistentes.

Incluyen:

1. Standing Instructions
2. Knowledge Base
3. Conversation History

#### Best Use Cases

- Trabajo recurrente
- Contexto estable
- Formato repetitivo

#### Rule of Thumb

Crear un Project cuando al menos dos de estas condiciones se cumplan:

- La tarea se repite
- El contexto es estable
- El formato de salida es consistente

---

### Artifacts

Entregables generados por Claude.

#### Examples

- Documentos
- Informes
- Código
- Tablas

#### Key Takeaway

Usar Artifacts cuando el resultado final será consumido por otras personas.

---

### Research

Investigación profunda basada en múltiples fuentes.

#### Best Use Cases

- Estudios de mercado
- Comparativas complejas
- Investigación técnica
- Información actualizada

#### Key Takeaway

Research va más allá de Web Search mediante síntesis multi-fuente.

---

### Context Management

El contexto se degrada con conversaciones largas.

#### Warning Signs

- Claude deja de seguir instrucciones previas
- Pierde continuidad
- Disminuye la precisión

#### Recommended Actions

##### Restart

Crear una conversación nueva.

##### Summarize

Generar un resumen y reutilizarlo como contexto inicial.

##### Persist

Guardar información en:

- Memory
- Project Knowledge Base

---

### Memory Management

La memoria debe mantenerse actualizada.

#### Best Practices

- Revisar periódicamente
- Eliminar datos obsoletos
- Actualizar información relevante

#### Key Takeaway

La calidad de las memorias importa más que la cantidad.

---

### Usage Limits

Los límites dependen de:

- Plan contratado
- Modelo utilizado
- Ventanas temporales de uso

#### Best Practices

- Dividir tareas grandes
- Guardar progreso
- Reiniciar con resúmenes

---

### Model Selection Principles

#### Opus

Elegir cuando:

- La calidad es prioritaria
- Existe ambigüedad
- El análisis es complejo
- El resultado tiene alto impacto

Trade-off:

Mayor calidad a cambio de menor velocidad y mayor coste.

---

### Code Execution

Utilizar cuando:

- Hay cálculos
- Hay datos estructurados
- La precisión es crítica

#### Typical Examples

- Finanzas
- Encuestas
- Reporting
- Análisis cuantitativo

---

## Summary

### Main Ideas

- Claude es probabilístico.
- La confianza no garantiza precisión.
- El contexto es limitado.
- El conocimiento tiene una fecha límite de entrenamiento.
- Existen distintos puntos de entrada según la tarea.
- Los Projects son útiles para trabajo recurrente.
- El contexto debe gestionarse activamente.
- Code Execution es la opción adecuada para cálculos.
- Opus es la opción para razonamiento complejo.

### Important Details

- Chat → trabajo puntual.
- Project → trabajo recurrente.
- Artifact → entregable.
- Research → investigación profunda.
- Restart, Summarize y Persist son las tres estrategias principales de gestión de contexto.

### Best Practices

- Verificar información crítica.
- Utilizar Projects para tareas repetitivas.
- Mantener la memoria actualizada.
- Reiniciar conversaciones largas cuando sea necesario.
- Persistir información importante en Knowledge Base.

---

## Personal Notes

- Este módulo es muy conceptual.
- Probables preguntas de examen relacionadas con:
  - Chat vs Project
  - Research vs Web Search
  - Context Window
  - Memory Management
  - Opus vs Sonnet
  - Code Execution

---

## Potential Exam Questions

## Potential Exam Questions

### Question 1

¿Por qué Claude puede generar respuestas diferentes cuando recibe exactamente la misma pregunta varias veces?

**Answer:**

Porque los modelos generativos producen respuestas de forma probabilística. No recuperan una respuesta fija desde una base de datos, sino que generan contenido basándose en probabilidades.

---

### Question 2

¿Por qué no debe utilizarse el tono de confianza de Claude como indicador de precisión?

**Answer:**

Porque Claude puede producir respuestas incorrectas con el mismo nivel de fluidez y seguridad que una respuesta correcta. La confianza no garantiza exactitud.

---

### Question 3

¿Qué significa la afirmación "Context is a budget"?

**Answer:**

Que la conversación dispone de una cantidad limitada de contexto. A medida que la sesión crece, parte del contenido anterior puede resumirse o perder relevancia.

---

### Question 4

¿Cuáles son las señales más comunes de degradación del contexto?

**Answer:**

- Claude deja de seguir instrucciones anteriores.
- Pierde continuidad respecto a decisiones previas.
- La precisión disminuye por pérdida de información relevante.

---

### Question 5

¿Cuáles son las tres estrategias principales para gestionar la degradación del contexto?

**Answer:**

- Restart
- Summarize
- Persist

---

### Question 6

¿Cuándo debería utilizarse un Project en lugar de un Chat?

**Answer:**

Cuando el trabajo es recurrente, el contexto permanece estable y/o el formato de salida suele repetirse entre sesiones.

---

### Question 7

¿Cuáles son los tres componentes principales de un Project?

**Answer:**

1. Standing Instructions
2. Knowledge Base
3. Conversation History

---

### Question 8

¿Cuándo merece la pena crear un Project?

**Answer:**

Cuando al menos dos de las siguientes condiciones se cumplen:

- La tarea es recurrente.
- El contexto es estable.
- El formato de salida es consistente.

---

### Question 9

¿Cuál es la diferencia principal entre Chat y Project?

**Answer:**

Chat está pensado para tareas puntuales. Project proporciona contexto persistente mediante instrucciones permanentes y una base de conocimiento reutilizable.

---

### Question 10

¿Cuándo debería utilizarse Research?

**Answer:**

Cuando el trabajo requiere investigación profunda, síntesis de múltiples fuentes o información actualizada.

---

### Question 11

¿Cuál es la diferencia entre Research y Web Search?

**Answer:**

Web Search realiza búsquedas puntuales. Research ejecuta búsquedas múltiples y sintetiza información procedente de varias fuentes.

---

### Question 12

¿Cuándo debería utilizarse un Artifact?

**Answer:**

Cuando el resultado es un entregable que será leído o utilizado posteriormente, como documentos, informes, tablas o código.

---

### Question 13

¿Cuándo es recomendable utilizar Code Execution?

**Answer:**

Cuando existen cálculos, análisis de datos o transformaciones donde la precisión es crítica.

---

### Question 14

¿Por qué los escenarios de análisis financiero y encuestas suelen requerir Code Execution?

**Answer:**

Porque implican cálculos sobre datos reales y la exactitud de los resultados es importante.

---

### Question 15

¿En qué tipo de situaciones debería seleccionarse Opus?

**Answer:**

En tareas complejas, ambiguas o de alto impacto donde la profundidad del razonamiento es más importante que la velocidad o el coste.

---

### Question 16

¿Cuál es el principal trade-off al elegir Opus?

**Answer:**

Mayor calidad de razonamiento a cambio de menor velocidad y mayor consumo de recursos.

---

### Question 17

¿Qué limitación impone la fecha de entrenamiento del modelo?

**Answer:**

Que Claude no puede garantizar conocimiento actualizado sobre eventos posteriores a dicha fecha sin acceso a fuentes recientes.

---

### Question 18

¿Dónde debería almacenarse la información que se utilizará repetidamente en futuras sesiones?

**Answer:**

En Memory o en la Knowledge Base de un Project.

---

### Question 19

¿Cuál es una buena práctica para mantener la calidad de Memory?

**Answer:**

Revisar periódicamente las entradas, eliminar información obsoleta y actualizar datos que hayan cambiado.

---

### Question 20

¿Qué conjunto de conceptos resume mejor este módulo?

**Answer:**

- Responses Vary
- Confidence ≠ Accuracy
- Context is a Budget
- Training Boundary
- Chat vs Project vs Artifact vs Research
- Restart / Summarize / Persist
- Code Execution
- Opus Trade-offs