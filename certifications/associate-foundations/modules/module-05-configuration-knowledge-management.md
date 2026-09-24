# Module 05 - Configuration & Knowledge Management

## Learning Objectives

- Configurar correctamente Claude Projects.
- Diferenciar entre instrucciones, conocimiento, Skills y Memory.
- Gestionar conectores y fuentes externas.
- Crear instrucciones persistentes efectivas.
- Mantener configuraciones, conocimientos y memorias actualizadas.
- Evitar degradación causada por configuraciones obsoletas.

---

## Key Concepts

### Operating Claude vs Using Claude

Existe una diferencia importante entre:

#### Using Claude

Realizar una buena consulta hoy.

#### Operating Claude

Configurar un entorno que produzca buenos resultados continuamente.

Esto incluye:

- Projects
- Instructions
- Knowledge Base
- Skills
- Memory

#### Key Takeaway

La configuración crea apalancamiento: se configura una vez y se utiliza muchas veces.

---

## Claude Project Configuration

Un Project está compuesto por cuatro mecanismos principales.

### 1. Standing Instructions

Definen comportamiento.

Ejemplos:

- Tono
- Formato
- Estándares de validación
- Reglas de verificación

#### Rule

Behavior → Instructions

#### Example

> Always cite sources and explicitly state uncertainty.

---

### 2. Knowledge Base

Define hechos y referencias.

Ejemplos:

- Políticas
- Documentación
- Manuales
- Brand Guides

#### Rule

Facts → Knowledge

#### Example

> Brand colors, procedures and official documentation.

---

### 3. Skills

Definen procedimientos reutilizables.

Ejemplos:

- Generación de informes
- Formateo de documentación
- Procesos repetitivos

#### Rule

Procedures → Skills

#### Important Note

Skills viven a nivel de cuenta y pueden reutilizarse entre Projects.

---

### 4. Scoped Memory

Mantiene continuidad dentro del Project.

Ejemplos:

- Decisiones previas
- Preferencias
- Stakeholders
- Contexto operativo

#### Rule

Continuity → Memory

#### Key Takeaway

Cada Project mantiene Memory aislada.

---

## Choosing the Correct Configuration Slot

### Standing Instructions

Utilizar para comportamiento.

Preguntarse:

> ¿Cómo debe comportarse Claude?

---

### Knowledge Base

Utilizar para información estable.

Preguntarse:

> ¿Qué necesita saber Claude?

---

### Skills

Utilizar para procesos repetibles.

Preguntarse:

> ¿Qué procedimiento debe seguir Claude?

---

### Scoped Memory

Utilizar para continuidad contextual.

Preguntarse:

> ¿Qué se ha aprendido o decidido dentro del proyecto?

---

## Common Configuration Mistakes

### Mistake 1

Guardar procedimientos en instrucciones.

#### Correct

Procedimientos → Skills

---

### Mistake 2

Guardar comportamiento en la Knowledge Base.

#### Correct

Comportamiento → Instructions

---

### Mistake 3

Guardar conocimiento permanente en Memory.

#### Correct

Información estable → Knowledge Base

---

## Project Example

### Client Workspace

#### Standing Instructions

- Formal tone
- Always cite sources
- Declare uncertainty

#### Knowledge Base

- Brand guide
- Statement of Work
- Previous reports

#### Skills

- Status report generation

#### Memory

- Stakeholder preferences
- Historical decisions

#### Benefit

Configuración consistente para todo el equipo.

---

## Scoped Memory

Memory es un mecanismo de primera clase.

### Knowledge Base Stores

Información estable.

Ejemplos:

- Políticas
- Templates
- Brand Guides

---

### Memory Stores

Información cambiante.

Ejemplos:

- Decisiones
- Preferencias
- Contexto reciente

---

### Key Takeaway

Knowledge = Facts

Memory = Evolving Context

---

## Pairing Configuration Mechanisms

Las mejores configuraciones suelen utilizar múltiples mecanismos.

### Example

#### Instruction

Always cite sources.

#### Knowledge Base

Contains source documents.

#### Result

Claude tiene documentos y reglas para utilizarlos.

### Key Takeaway

Muchos requisitos requieren dos mecanismos trabajando juntos.

---

## Connectors

Los conectores permiten acceder a sistemas externos.

### Examples

- Google Drive
- Gmail

### Purpose

Permitir acceso controlado a información existente.

---

## Connector Boundaries

Cada conector tiene capacidades específicas.

### Important Principle

No asumir capacidades no documentadas.

#### Example

Un conector de correo puede:

✅ Leer mensajes

✅ Buscar mensajes

❌ Enviar mensajes

---

### Key Takeaway

Muchos errores son expectativas incorrectas, no fallos del conector.

---

## Connector Pitfalls

### Wrong Connector Source

Conectar una fuente no aprobada.

#### Recommendation

Confirmar la ruta correcta con el administrador.

---

### Boundary Confusion

Asumir capacidades inexistentes.

#### Impact

Incidencias mal clasificadas y diagnósticos incorrectos.

---

## Managing Uploaded Knowledge

La Knowledge Base requiere mantenimiento.

### Best Practices

#### Remove Duplicates

Evitar múltiples versiones del mismo documento.

---

#### Remove Deprecated Material

Eliminar documentación obsoleta.

---

#### Keep Sources Current

Actualizar contenido regularmente.

---

### Key Takeaway

Knowledge Bases desorganizadas degradan la calidad de respuesta.

---

## System-Level Instructions

Las instrucciones persistentes eliminan la necesidad de repetir reglas.

### Good Use Cases

- Citation requirements
- Verification rules
- Formatting standards
- Tone guidelines

---

### Characteristics of Good Instructions

#### Specific

✅ Good

> Cite every figure and mark uncertain values as unverified.

❌ Bad

> Be accurate.

---

### Precision Principle

Las instrucciones vagas fallan silenciosamente.

#### Key Takeaway

La precisión produce consistencia.

---

## Configuration Maintenance

Las configuraciones envejecen.

Sin mantenimiento:

- Skills quedan obsoletas.
- Memory se degrada.
- Knowledge queda desactualizada.
- Instructions dejan de reflejar los procesos actuales.

---

## Review Cadence

### Recommendation

Revisión mensual para Projects activos.

### Review Checklist

- Instructions actualizadas
- Knowledge vigente
- Skills correctas
- Memory relevante

---

## Skills Lifecycle

### Organization Skills

Actualización automática.

---

### Custom Skills

Requieren actualización manual.

### Risk

Configuraciones incorrectas pueden degradar la salida sin producir errores visibles.

---

## Memory Lifecycle

### Best Practices

- Revisar periódicamente.
- Eliminar contexto obsoleto.
- Mantener solo información útil.

### Key Takeaway

La calidad de Memory importa más que el volumen.

---

## Configuration Drift

La degradación suele producirse silenciosamente.

### Symptoms

- Formatos incorrectos.
- Información antigua.
- Referencias inconsistentes.
- Calidad decreciente.

---

### Example

El proyecto sigue utilizando:

- Métricas antiguas.
- Plantillas obsoletas.
- Stakeholders que ya no existen.

### Fix

Actualizar:

- Instructions
- Knowledge Base
- Memory

No necesariamente el prompt.

---

## Summary

### Main Ideas

- Configurar Claude correctamente mejora todas las conversaciones futuras.
- Projects utilizan Instructions, Knowledge, Skills y Memory.
- Cada mecanismo tiene una finalidad distinta.
- Los conectores tienen límites claros.
- Las instrucciones deben ser específicas.
- La configuración requiere mantenimiento continuo.

### Important Details

- Behavior → Instructions
- Facts → Knowledge
- Procedures → Skills
- Continuity → Memory

### Best Practices

- Mantener las configuraciones actualizadas.
- Revisar Projects mensualmente.
- Evitar duplicados.
- Separar clientes en Projects distintos.
- Utilizar instrucciones precisas.

---

## Exam Hot Topics

- Configuration vs Prompting
- Standing Instructions
- Knowledge Base
- Skills
- Scoped Memory
- Connectors
- Connector Boundaries
- Persistent Instructions
- Configuration Maintenance
- Configuration Drift
- Memory Lifecycle
- Skills Lifecycle

---

## Potential Exam Questions

### Question 1

¿Cuál es la diferencia entre usar Claude y operar Claude?

**Answer:** Operar Claude implica configurar y mantener un entorno reutilizable mediante Projects, Knowledge, Skills e Instructions.

---

### Question 2

¿Qué tipo de información pertenece a Standing Instructions?

**Answer:** Reglas de comportamiento y formato.

---

### Question 3

¿Qué tipo de información pertenece a la Knowledge Base?

**Answer:** Hechos, referencias y documentación.

---

### Question 4

¿Qué representan las Skills?

**Answer:** Procedimientos reutilizables.

---

### Question 5

¿Qué representa Scoped Memory?

**Answer:** Continuidad contextual dentro de un Project.

---

### Question 6

¿Dónde deberían almacenarse las preferencias de stakeholders?

**Answer:** Scoped Memory.

---

### Question 7

¿Dónde debería almacenarse un Brand Guide?

**Answer:** Knowledge Base.

---

### Question 8

¿Dónde debería configurarse una regla de citación obligatoria?

**Answer:** Standing Instructions.

---

### Question 9

¿Qué error común ocurre al utilizar una Knowledge Base?

**Answer:** Mantener múltiples versiones del mismo documento.

---

### Question 10

¿Por qué deben mantenerse actualizadas las configuraciones?

**Answer:** Porque la degradación es silenciosa.

---

### Question 11

¿Dónde viven las Skills?

**Answer:** A nivel de cuenta.

---

### Question 12

¿Cuál es el propósito de Scoped Memory?

**Answer:** Mantener continuidad aislada por proyecto.

---

### Question 13

¿Qué es Configuration Drift?

**Answer:** La degradación causada por configuraciones desactualizadas.

---

### Question 14

¿Qué se recomienda para Projects activos?

**Answer:** Revisiones mensuales.

---

### Question 15

¿Qué debe hacerse con documentación obsoleta?

**Answer:** Eliminarla o actualizarla.

---

### Question 16

¿Qué son los Connectors?

**Answer:** Integraciones controladas con sistemas externos.

---

### Question 17

¿Todos los conectores pueden realizar cualquier acción?

**Answer:** No. Cada conector tiene límites definidos.

---

### Question 18

¿Qué caracteriza una buena instrucción persistente?

**Answer:** Precisión y claridad.

---

### Question 19

¿Qué es más importante en Memory?

**Answer:** Calidad y actualidad.

---

### Question 20

¿Cuál es la regla más importante del módulo?

**Answer:** Colocar cada necesidad en el mecanismo adecuado: Instructions, Knowledge, Skills o Memory.

---

## Flashcards

Q: Behavior goes where?

A: Standing Instructions.

Q: Facts go where?

A: Knowledge Base.

Q: Procedures go where?

A: Skills.

Q: Continuity goes where?

A: Scoped Memory.

Q: What is Configuration Drift?

A: Silent degradation caused by stale configuration.

Q: How often should active Projects be reviewed?

A: Monthly.

Q: Where do Skills live?

A: Account level.

Q: What do Connectors provide?

A: Controlled access to external systems.

Q: What is the most common configuration mistake?

A: Putting information in the wrong configuration slot.

Q: What is the core principle of the module?

A: Configure once, benefit many times.

---

## Review Status

- [x] Reviewed once
- [ ] Reviewed twice
- [ ] Included in final cheatsheet