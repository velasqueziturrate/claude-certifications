# Module 06 - Governance, Risk & Responsible Use

## Learning Objectives

- Identificar casos de uso apropiados e inapropiados para Claude.
- Aplicar criterios de sensibilidad de datos, privacidad y regulación.
- Evaluar riesgos asociados a Skills, conectores y capacidades.
- Aplicar políticas organizativas de IA de forma consistente.
- Identificar riesgos éticos relacionados con sesgo, equidad y transparencia.
- Comprender los principios de gobernanza responsable en el uso de IA.

---

## Key Concepts

### Governance Is a Practitioner Skill

La gobernanza no es únicamente una política corporativa.

La gobernanza ocurre en cada decisión diaria:

- Qué dato subir.
- Qué Skill habilitar.
- Qué caso de uso aprobar.
- Qué control aplicar.

### Key Takeaway

La adopción segura de IA depende del criterio de los usuarios, no únicamente de las políticas.

---

## Core Competencies

Dos competencias dominan este módulo:

### Diligence

Responsabilidad, validación y cumplimiento continuo.

### Delegation

Capacidad de decidir qué trabajo puede realizar IA, qué requiere revisión humana y qué debe permanecer completamente en manos humanas.

---

## Appropriate vs Inappropriate Use Cases

Determinar si un caso de uso es adecuado requiere un análisis estructurado.

No debe realizarse por intuición.

---

## Delegation Criteria for Screening Use Cases

### 1. Reversibility

Pregunta:

> ¿Puede corregirse el error antes de causar daño?

#### Rule

Mayor reversibilidad → mayor posibilidad de delegación.

---

### 2. Consequence of Error

Pregunta:

> ¿Cuál es el impacto del error?

#### Rule

Mayor impacto → mayor control humano.

---

### 3. Need for Human Creativity or Empathy

Pregunta:

> ¿Requiere empatía, juicio humano o relación interpersonal?

#### Rule

Algunas tareas deben seguir siendo humanas independientemente de la capacidad de la IA.

---

### 4. Accountability

Pregunta:

> ¿Quién es responsable del resultado?

#### Rule

La responsabilidad nunca se transfiere a Claude.

---

## The Load-Bearing Criterion

No todos los criterios pesan igual en todos los casos.

El criterio más importante recibe el nombre de:

### Load-Bearing Criterion

Es el criterio que cambiaría completamente la clasificación del caso de uso.

### Exam Note

Identificar el criterio dominante convierte una decisión en defendible frente a auditoría o compliance.

---

## Three Use Case Classifications

### Fully Appropriate

Características:

- Reversible.
- Bajo impacto.
- No requiere juicio humano especial.

Ejemplo:

- Crear FAQs internas basadas en documentación aprobada.

---

### Appropriate With Human Review

Características:

- Claude aporta valor.
- Existe un control humano explícito.

Ejemplo:

- Generar borradores de respuesta al cliente.
- Cribado inicial de currículums.

---

### Inappropriate

Características:

- Consecuencias irreversibles.
- Accountability no transferible.
- Alto impacto.

Ejemplos:

- Diagnósticos médicos definitivos.
- Determinaciones legales finales.
- Decisiones finales sobre elegibilidad de beneficios.

---

## Human Review Gates

Una revisión humana válida debe responder tres preguntas.

### Who

¿Quién revisa?

---

### What

¿Qué verifica?

---

### When

¿Cuándo ocurre la revisión?

---

### Bad Example

> Human in the loop.

---

### Good Example

> Hiring manager reviews the shortlist before any candidate is contacted.

### Key Takeaway

Un gate indefinido no es realmente un control.

---

## Skill Trust & Feature-Level Risk

### Core Principle

Un Skill es software.

Debe evaluarse igual que cualquier software corporativo.

---

## Skill Trust Evaluation

### 1. Source

Pregunta:

> ¿Quién publicó el Skill?

#### Trust Order

1. Anthropic
2. Organización
3. Terceros conocidos
4. Fuente desconocida

---

### 2. Reach

Pregunta:

> ¿A qué datos o herramientas podría acceder?

### Important Insight

Los Skills heredan los permisos de la sesión donde se ejecutan.

---

### 3. Appropriateness

Pregunta:

> ¿Es realmente la herramienta adecuada para el trabajo?

---

## Three Trust Outcomes

### Enable

Fuente, alcance y propósito adecuados.

---

### Escalate

Requiere revisión de administración o seguridad.

---

### Decline

Fuente dudosa o permisos claramente excesivos.

---

## Least Privilege Principle

Regla general:

> Conceder únicamente el acceso mínimo necesario.

### Exam Note

Aplica a:

- Skills
- Connectors
- Integraciones
- Herramientas

---

## Data Sensitivity & Privacy

Antes de utilizar cualquier funcionalidad:

### Classify First

Clasificar la sensibilidad de los datos.

---

## Data Classification

### Green

Seguro para utilizar.

Ejemplos:

- Información pública.
- Datos agregados.
- Datos anonimizados.

---

### Yellow

Requiere revisión previa.

Ejemplos:

- Documentación interna.
- Datos de contacto.
- Información confidencial no regulada.

---

### Red

No utilizar sin una ruta aprobada.

Ejemplos:

- Datos regulados.
- Datos de salud.
- Información financiera protegida.
- Credenciales.
- Secretos.

---

## Redaction & Anonymization

Si la identidad no es necesaria para el análisis:

Eliminar:

- Nombres.
- Cuentas.
- IDs.
- Identificadores personales.

---

## Redaction Failure Modes

### Partial Redaction

Eliminar solo parte de los identificadores.

Resultado:

La persona sigue siendo identificable.

---

### Redaction That Breaks The Task

Eliminar información necesaria para realizar el trabajo.

Resultado:

El análisis deja de ser válido.

---

## Feature Controls

### Code Execution Sandbox

Los archivos se procesan en un entorno aislado.

#### Best Practice

Revisar cuidadosamente los datos antes de procesarlos.

---

### Memory Persistence

La información puede persistir entre sesiones.

#### Risk

Retener información sensible innecesariamente.

---

### Incognito Mode

Evita:

- Historial.
- Memoria.

### Important Exam Point

Incognito NO convierte automáticamente información sensible en información segura.

---

### Organization-Level Memory Controls

La organización puede controlar:

- Activación de memoria.
- Persistencia.
- Configuración global.

---

## Core Rule

Clasificar primero.

Elegir el control adecuado después.

---

## Incognito Limitation

### Key Principle

Incognito controla persistencia.

NO valida si un dato está autorizado para utilizarse.

### Exam Note

Datos regulados siguen requiriendo aprobación incluso en Incognito.

---

## Organizational Policies & Diligence

### Governance Is A Habit

El cumplimiento debe aplicarse continuamente.

No solo en casos de alto riesgo.

---

## Audit Usage Against Policy

Revisar periódicamente:

- Casos de uso.
- Datos cargados.
- Skills habilitados.
- Gates de revisión.

---

## Common Governance Drift

### Examples

- Datos cargados en ubicaciones no aprobadas.
- Skills habilitados sin revisión.
- Gates de revisión omitidos.

### Key Takeaway

La mayoría de incumplimientos no son maliciosos.

Son hábitos incorrectos acumulados.

---

## Stay Current

Tanto las capacidades como las políticas evolucionan.

### Best Practice

Mantenerse actualizado respecto a:

- Nuevas políticas.
- Nuevas funcionalidades.
- Nuevos riesgos.

---

## Ethical Implications

Los riesgos éticos suelen estar ocultos en resultados aparentemente normales.

---

## Bias

La salida puede contener sesgo procedente de:

- Prompts.
- Framing.
- Patrones del modelo.

### High-Risk Areas

- Contratación.
- Evaluación de personas.
- Comunicaciones sensibles.

---

## Fairness

Pregunta:

> ¿Se trata a todas las personas de forma equitativa?

### Key Takeaway

Los procesos que afectan a personas requieren revisión adicional.

---

## Transparency & Disclosure

Saber cuándo debe comunicarse el uso de IA.

### Rule

Si existe duda:

Disclose rather than conceal.

---

## Ethical Reasoning Framework

Preguntas clave:

1. ¿Quién resulta afectado?
2. ¿Qué puede salir mal?
3. ¿Qué resultado sería justo?
4. ¿Qué nivel de transparencia se requiere?

---

## Escalation Principle

Cuando el impacto potencial supera el criterio individual:

Escalar.

Ejemplos:

- Grandes poblaciones afectadas.
- Daños importantes.
- Cuestiones éticas complejas.

---

## Performance Review Example

Caso:

Un manager utiliza Claude para redactar evaluaciones de desempeño.

### Correct Classification

Appropriate With Human Review.

### Required Controls

- Revisión humana.
- Verificación de equidad.
- Comprobación de consistencia.

---

## Key Takeaways

### 1. Governance Is a Practitioner Skill

La gobernanza se aplica decisión a decisión.

---

### 2. Screen Use Cases With Delegation Criteria

Utilizar:

- Reversibility
- Consequence
- Human Element
- Accountability

---

### 3. A Skill Is Software

Evaluar Skills igual que cualquier software corporativo.

---

### 4. Understand Data Sensitivity Before Uploading

Clasificar primero.

Aplicar controles después.

---

### 5. Ethical Risk Hides In Ordinary Outputs

Revisar:

- Bias
- Fairness
- Disclosure

como parte del proceso habitual.

---

## Summary

### Main Ideas

- La gobernanza es una práctica diaria.
- Los casos de uso deben clasificarse correctamente.
- Los Skills requieren evaluación de confianza.
- La sensibilidad de datos determina el tratamiento adecuado.
- Incognito no sustituye la clasificación de datos.
- La diligencia implica auditar y corregir desviaciones.
- El sesgo y la equidad deben evaluarse explícitamente.
- La transparencia es parte del uso responsable.

### Important Details

- Reversibility
- Consequence
- Human Element
- Accountability
- Load-Bearing Criterion
- Trust Evaluation
- Green / Yellow / Red Data
- Least Privilege
- Incognito
- Disclosure

### Best Practices

- Clasificar antes de cargar datos.
- Definir gates explícitos.
- Auditar Skills antes de habilitarlos.
- Evaluar sesgo en trabajos que afectan personas.
- Escalar cuestiones éticas complejas.
- Mantener cumplimiento continuo.

---

## Personal Notes

### Fórmulas de examen

Use Case Classification:

Reversibility + Consequence + Human Element + Accountability

Skill Trust:

Source + Reach + Appropriateness

Data Handling:

Classify → Control → Verify

Ethics:

Bias + Fairness + Transparency

---

## Exam Hot Topics

- Governance
- Diligence
- Delegation
- Use Case Classification
- Human Review Gates
- Skill Trust
- Least Privilege
- Data Classification
- Incognito
- Privacy
- Governance Drift
- Bias
- Fairness
- Disclosure
- Ethical Escalation

---

## Potential Exam Questions

### Question 1

¿Cuáles son las dos competencias centrales del módulo?

**Answer:** Diligence y Delegation.

---

### Question 2

¿Qué cuatro criterios se utilizan para evaluar casos de uso?

**Answer:** Reversibility, Consequence, Human Element y Accountability.

---

### Question 3

¿Qué es un Load-Bearing Criterion?

**Answer:** El criterio que determina la clasificación final del caso de uso.

---

### Question 4

¿Cuáles son las tres clasificaciones posibles de un caso de uso?

**Answer:** Fully Appropriate, Appropriate With Human Review e Inappropriate.

---

### Question 5

¿Qué debe definir un Human Review Gate?

**Answer:** Who, What y When.

---

### Question 6

¿Por qué un Skill debe tratarse como software?

**Answer:** Porque puede acceder a datos y herramientas disponibles en la sesión.

---

### Question 7

¿Qué tres elementos forman un Skill Trust Check?

**Answer:** Source, Reach y Appropriateness.

---

### Question 8

¿Qué significa Least Privilege?

**Answer:** Conceder únicamente los permisos mínimos necesarios.

---

### Question 9

¿Cuáles son las tres categorías de sensibilidad de datos?

**Answer:** Green, Yellow y Red.

---

### Question 10

¿Qué debe hacerse cuando existe duda entre dos niveles de sensibilidad?

**Answer:** Tratar el dato como el más sensible.

---

### Question 11

¿Qué es una redacción parcial insuficiente?

**Answer:** Eliminar algunos identificadores manteniendo otros que permiten identificar a la persona.

---

### Question 12

¿Qué hace Incognito?

**Answer:** Evita historial y memoria.

---

### Question 13

¿Por qué Incognito no resuelve todos los problemas de privacidad?

**Answer:** Porque no valida si el uso de los datos está permitido.

---

### Question 14

¿Qué significa Governance Drift?

**Answer:** Desviación gradual entre política y práctica.

---

### Question 15

¿Para qué sirven las auditorías de uso?

**Answer:** Detectar y corregir desviaciones de política.

---

### Question 16

¿Qué riesgos éticos deben revisarse rutinariamente?

**Answer:** Bias, Fairness y Transparency.

---

### Question 17

¿Qué hacer cuando existe duda sobre divulgación de uso de IA?

**Answer:** Disclose rather than conceal.

---

### Question 18

¿Cuándo debe escalarse una cuestión ética?

**Answer:** Cuando supera el ámbito de decisión individual.

---

### Question 19

¿Cómo debe clasificarse un diagnóstico médico final generado por IA?

**Answer:** Inappropriate.

---

### Question 20

¿Cuál es la regla más importante del módulo?

**Answer:** Governance is a practitioner skill.

---

## Flashcards

Q: ¿Qué competencias dominan el módulo?

A: Diligence y Delegation.

---

Q: ¿Qué cuatro criterios se utilizan para evaluar casos de uso?

A: Reversibility, Consequence, Human Element y Accountability.

---

Q: ¿Qué es un Load-Bearing Criterion?

A: El criterio que más influye en la clasificación final.

---

Q: ¿Cómo se evalúa un Skill?

A: Source + Reach + Appropriateness.

---

Q: ¿Qué significa Least Privilege?

A: Dar únicamente los permisos necesarios.

---

Q: ¿Cuáles son las categorías de sensibilidad?

A: Green, Yellow y Red.

---

Q: ¿Qué hace Incognito?

A: Evita historial y memoria.

---

Q: ¿Qué no hace Incognito?

A: No autoriza el uso de datos regulados.

---

Q: ¿Qué riesgos éticos deben revisarse siempre?

A: Bias, Fairness y Transparency.

---

Q: ¿Cuál es la idea principal del módulo?

A: Responsible use is exercised one decision at a time.

---

## Review Status

- [x] Reviewed once
- [ ] Reviewed twice
- [ ] Included in final cheatsheet