# Module 03 - Evaluating & Validating Claude's Output

## Learning Objectives

- Evaluar la calidad de los resultados generados por Claude.
- Identificar errores, omisiones y señales de alucinación.
- Aplicar técnicas de verificación y grounding.
- Determinar cuándo la revisión humana es obligatoria.
- Adaptar resultados según audiencia y nivel de riesgo.
- Seleccionar formatos de salida adecuados según la fiabilidad requerida.

---

## Key Concepts

### Accountability Stays With You

Claude ayuda a generar contenido, pero la responsabilidad final permanece en el usuario.

#### Key Takeaway

Todo lo que se entrega sigue siendo responsabilidad profesional del usuario.

---

### Evaluate Against Three References

Toda evaluación debe contrastar:

#### Requirements

¿Responde realmente a la petición?

#### Source Material

¿Está soportado por las fuentes?

#### Professional Standards

¿Cumple el nivel de calidad esperado?

#### Key Takeaway

Precisión, completitud y calidad profesional son verificaciones distintas.

---

### Accuracy vs Completeness

Una respuesta puede ser:

✅ Correcta

❌ Incompleta

#### Accuracy

Verifica si lo incluido es correcto.

#### Completeness

Verifica si falta información importante.

#### Key Takeaway

La precisión no garantiza completitud.

---

### Common Failure Patterns

#### Fabricated Specifics

Datos concretos inventados que parecen legítimos.

Ejemplo:

- Estadísticas precisas sin fuente.
- Números aparentemente exactos.

---

#### Confident Uncertainty

Información incierta presentada con autoridad.

---

#### Completeness Gaps

Información relevante omitida.

#### Key Takeaway

Plausible no significa verificado.

---

## Fact-Checking Techniques

### Allow "I Don't Know"

Permitir explícitamente que Claude admita incertidumbre.

#### Example

> If the answer is not supported by the provided materials, say so explicitly.

#### Benefit

Reduce la invención de contenido.

---

### Restrict to Sources

Limitar respuestas únicamente a documentos proporcionados.

#### Example

> Use only the attached contract.

#### Benefit

Convierte generación abierta en recuperación controlada.

---

### Require Auditable Citations

Solicitar referencias rastreables.

#### Example

> Cite the exact section and clause supporting each claim.

#### Benefit

Facilita la validación.

---

### Verification Checklist

Antes de utilizar una respuesta:

- ¿Permití incertidumbre?
- ¿Restringí las fuentes?
- ¿Solicité citas verificables?
- ¿Validé afirmaciones críticas?

#### Key Takeaway

Es más eficiente prevenir errores que detectarlos después.

---

## Grounding Techniques

### Quote First, Then Analyze

1. Extraer citas relevantes.
2. Analizar únicamente esas citas.

#### Benefit

La evidencia queda visible.

---

### Best-of-N Comparison

Ejecutar varias veces la misma petición.

#### Interpretation

Coincidencia → aumenta confianza.

Diferencia → requiere revisión humana.

---

### Validate Against Authoritative Sources

Nunca validar únicamente con otra respuesta de Claude.

Validar mediante:

- Documentación oficial.
- Fuentes regulatorias.
- Sistemas corporativos.
- Datos originales.

#### Key Takeaway

La segunda opinión debe ser una fuente autorizada.

---

## Human Review & Due Diligence

### Core Principle

La responsabilidad no se transfiere a Claude.

#### Key Takeaway

La IA asiste; la responsabilidad permanece.

---

## Four Risk Thresholds

### Stakes

¿Cuál es el coste de un error?

---

### Reversibility

¿Puede deshacerse la acción?

---

### Audience

¿Quién verá el contenido?

---

### Regulatory Exposure

¿Existe regulación aplicable?

---

### Risk Rule

Cuanto mayores sean estos factores, más necesaria será la revisión humana.

---

## Always Review Categories

### Client Deliverables

Entregables finales para clientes.

---

### Financial Calculations

Contenido financiero o auditado.

---

### Regulated Information

Datos regulados o sensibles.

---

### Legal & Public Communications

Contenido con consecuencias legales o reputacionales.

---

## Iteration vs Escalation

### Iteration

Cada ronda mejora claramente el resultado.

---

### Escalation

Las mejoras se vuelven marginales.

#### Signal

Rendimientos decrecientes.

#### Action

Escalar a revisión humana.

#### Key Takeaway

Más prompting no siempre genera mejores resultados.

---

## Editing & Adapting Output

### Three Editing Passes

#### 1. Clarity

Eliminar:

- Repetición
- Ambigüedad
- Ruido

---

#### 2. Tone

Adaptar el lenguaje a:

- Compañeros
- Clientes
- Ejecutivos
- Reguladores

---

#### 3. Formatting

Adaptar la estructura de lectura.

##### Executive

Breve y orientado a decisiones.

##### Operational

Detallado y accionable.

##### External

Formal y preciso.

---

## Audience Calibration

Los hechos permanecen iguales.

Lo que cambia:

- Profundidad
- Tono
- Estructura
- Nivel de detalle

### Executive Audience

Decisión e impacto.

### Working Team

Método y ejecución.

### External Audience

Precisión y control del mensaje.

---

## Output Formats

### Inline

Respuestas rápidas dentro del chat.

---

### Artifacts

Documentos e informes reutilizables.

---

### Structured Formats

Tablas y estructuras de datos.

---

### Code Execution

Resultados calculados y verificables.

#### Key Takeaway

La elección del formato es una decisión de fiabilidad.

---

## Code Execution Validation

### Prose Path

Produce una estimación plausible.

---

### Code Execution Path

Produce un resultado calculado.

#### Benefits

- Repetible
- Auditable
- Verificable

#### Key Takeaway

Cuando los números importan, utilizar Code Execution.

---

## Input Curation

### Remove Duplicates

Eliminar documentos redundantes.

---

### Label Sources

Identificar claramente cada fuente.

---

### Remove Noise

Eliminar material irrelevante.

#### Principle

Ruido de entrada → ruido de salida.

---

## Output Triage Framework

### Ready to Use

- Riesgo bajo
- Uso interno
- Correcciones menores

---

### Needs Revision

- Inconsistencias
- Falta validación
- Información insuficiente

---

### Needs Human Override

- Regulación
- Alto impacto
- Consecuencias externas

---

## Exam Hot Topics

- Accountability
- Accuracy vs Completeness
- Fabricated Specifics
- Allow Uncertainty
- Source Restriction
- Auditable Citations
- Grounding
- Best-of-N
- Human Review
- Risk Thresholds
- Audience Calibration
- Output Formats
- Code Execution
- Input Curation
- Triage Framework

---

## Summary

### Main Ideas

- La responsabilidad final es humana.
- Accuracy y Completeness son verificaciones distintas.
- La mejor validación empieza en el prompt.
- Las citas verificables mejoran la confianza.
- Grounding conecta conclusiones con evidencia.
- Los resultados de alto riesgo requieren revisión humana.
- Los formatos deben elegirse según la fiabilidad necesaria.
- Code Execution es obligatorio para cálculos importantes.

### Important Details

- Allow uncertainty.
- Restrict sources.
- Require citations.
- Verify against authoritative sources.
- Review high-risk outputs.
- Curate inputs.

### Best Practices

- No confiar en la fluidez.
- Validar afirmaciones críticas.
- Revisar entregables externos.
- Utilizar evidencia verificable.
- Escalar cuando la iteración deja de aportar valor.

---

## Personal Notes

### Fórmula rápida para examen

Requirements + Source Material + Professional Standards

Accuracy + Completeness

Allow Uncertainty + Source Restriction + Auditable Citations

Stakes + Reversibility + Audience + Regulatory Exposure

---

## Potential Exam Questions

### Question 1

¿Quién es responsable del contenido final generado con Claude?

**Answer:** El usuario.

### Question 2

¿Cuáles son las tres referencias principales para evaluar una salida?

**Answer:** Requirements, Source Material y Professional Standards.

### Question 3

¿Qué diferencia existe entre Accuracy y Completeness?

**Answer:** Accuracy valida corrección; Completeness valida que no falte información importante.

### Question 4

¿Qué es un Fabricated Specific?

**Answer:** Un dato inventado que aparenta autoridad por su precisión.

### Question 5

¿Por qué una respuesta segura no implica que sea correcta?

**Answer:** Porque la confianza no es evidencia.

### Question 6

¿Qué técnica reduce alucinaciones permitiendo admitir incertidumbre?

**Answer:** Allow "I don't know".

### Question 7

¿Qué técnica obliga a Claude a utilizar únicamente material proporcionado?

**Answer:** Source Restriction.

### Question 8

¿Qué son las Auditable Citations?

**Answer:** Referencias rastreables y verificables.

### Question 9

¿En qué consiste Quote First, Then Analyze?

**Answer:** Extraer evidencia antes de analizar.

### Question 10

¿Qué es Best-of-N?

**Answer:** Comparar varias ejecuciones de la misma solicitud.

### Question 11

¿Con qué debe validarse una afirmación crítica?

**Answer:** Con fuentes autorizadas.

### Question 12

¿Cuáles son los cuatro Risk Thresholds?

**Answer:** Stakes, Reversibility, Audience y Regulatory Exposure.

### Question 13

¿Qué tipo de trabajo requiere siempre revisión humana?

**Answer:** Entregables críticos, financieros, legales o regulatorios.

### Question 14

¿Cuándo debe escalarse un resultado a revisión humana?

**Answer:** Cuando el riesgo es alto o la iteración deja de mejorar el resultado.

### Question 15

¿Qué prioriza una audiencia ejecutiva?

**Answer:** Decisiones e impacto.

### Question 16

¿Qué prioriza una audiencia operativa?

**Answer:** Detalle y ejecución.

### Question 17

¿Cuándo debe utilizarse Code Execution?

**Answer:** Cuando la precisión numérica es importante.

### Question 18

¿Qué es Input Curation?

**Answer:** Organizar, depurar y etiquetar las fuentes antes del análisis.

### Question 19

¿Qué significa Needs Revision dentro del Triage Framework?

**Answer:** Que la salida necesita correcciones antes de utilizarse.

### Question 20

¿Qué concepto resume mejor el objetivo del módulo?

**Answer:** Verificar y validar antes de confiar en cualquier resultado generado por IA.

---

## Flashcards

Q: ¿Quién es responsable de una salida de Claude?

A: El usuario.

Q: ¿Qué significa Accuracy?

A: Verificar que lo incluido sea correcto.

Q: ¿Qué significa Completeness?

A: Verificar que no falte información relevante.

Q: ¿Qué es un Fabricated Specific?

A: Un dato inventado que parece real.

Q: ¿Cómo se reducen las alucinaciones?

A: Allow Uncertainty + Source Restriction + Citations.

Q: ¿Qué es Grounding?

A: Vincular conclusiones con evidencia verificable.

Q: ¿Cuál es la mejor validación para afirmaciones críticas?

A: Fuentes autorizadas.

Q: ¿Cuáles son los Risk Thresholds?

A: Stakes, Reversibility, Audience y Regulatory Exposure.

Q: ¿Cuándo usar Code Execution?

A: Cuando los números importan.

Q: ¿Qué es Input Curation?

A: Limpiar y organizar las fuentes antes del análisis.

---

## References

- Associate Foundations Training Material
- Anthropic Documentation
