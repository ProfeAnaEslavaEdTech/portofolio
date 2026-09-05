# MLLDE y el tutor por voz: desarrollo y los tres tiers de evidencia
## Componente de la propuesta de investigación doctoral

**Autora:** Ana Eslava-Graterol — MLLDE (Universitat Politècnica de València)
**Objeto:** el **Módulo de Medición MLLDE** y su instanciación en un **tutor de inglés de negocios por
voz** (TK Coach / «Capi», Talketika), con un modelo de medición de pronunciación **por tres tiers de
evidencia**. **Fecha:** 2026-09-05.

---

## Resumen

Esta propuesta sitúa una **contribución metodológica**: cómo convertir la **producción oral real** de un
aprendiz frente a un agente de IA en **evidencia de competencia trazable al MCER**, sin que un modelo
generativo —fluido por diseño— **invente** una calificación. El aporte replicable es la separación
**motor + pack** (las reglas de medición no cambian por cliente; cada app rellena un pack) y una **política
de honestidad de la evidencia** organizada en **tres tiers** que evita reclamar más precisión que la que el
sistema realmente tiene. La pronunciación —la señal más difícil de medir— es el caso testigo: se desarrolla
por tiers, de lo medible hoy a la evaluación fonémica de investigación.

---

## 1. MLLDE — el método y el módulo de medición

**MLLDE** (Multimodal Language Learning Design & Evaluation) es el marco de la autora. Su **Módulo de
Medición** operacionaliza una idea central, *Measure ≠ Decide*:

- **El modelo observa; el motor decide.** La IA *describe* lo que ocurre en una interacción; un **motor
  determinista** (código) *computa* la banda a partir de esas observaciones. Nada en pantalla se inventa.
- **Anclaje al MCER.** No hay métrica sin descriptor: cada métrica cita una escala nombrada del *Companion
  Volume* (Consejo de Europa, 2020) y su identificador (IRI) en un **registry** único.
- **Escala 0–10** (pass ≥6, pisos ≥4; vista Cambridge 0–5 = round/2).
- **Motor + pack.** Las reglas (el motor) son client-agnósticas; cada producto rellena un **pack** (sus
  tareas, niveles, inventario de sonidos). Aplicar el módulo a una segunda app es *rellenar un pack, no
  rediseñar* — la promesa de replicabilidad que sostiene la tesis.
- **Cinco destrezas.** Recepción, producción, interacción y **mediación** (5.ª destreza, decisión 2026-08-04),
  todas ancladas al *Companion Volume*.
- **Trazabilidad y honestidad.** Toda la evidencia se registra como **xAPI** en un **LRS**; cada afirmación
  derivada de voz declara su **tier de evidencia** (ver §3) y su **modelo de medición** por sesión.

## 2. El tutor por voz (Capi) — arquitectura

El aprendiz practica **hablando** situaciones reales de trabajo con «Capi». El bucle de medición:

**Capi (role-play)** → **Evaluador MLLDE** (banda 0–10 + descriptor débil *i+1*) → **Práctica** (drills,
tarjetas, mediación) → **Capi** → la banda sube **en la siguiente conversación**.

- **Tres agentes que observan** (Capi · corrector · evaluador) + un **consolidador de código** (no un 4.º
  LLM) que computa el nivel acumulativo (`Global×5 + analíticas×2 ÷ pool × 10`) y emite una sola entrada al
  LRS. Un **redactor** escribe el resumen (no mide). Los **generadores** crean contenido (el código elige el
  descriptor, el LLM redacta).
- **Dos flujos, nunca cruzados:** *medición* (una vez por sesión: `completed` + rúbrica) y *pedagogía* (por
  turno: `adapted` + `pedagogical-action` + `learning-target`). La corrección es pedagogía y **nunca
  puntúa** (cortafuegos).
- **Feedback §10 + noticing.** El **código** decide el nivel de feedback (0–3); el **LLM** detecta y redacta.
  Dentro del recast, la **escala de noticing (0–4)** dosifica la *saliencia* según el nivel CEFR (modelar
  A2–B1 · elicitar B2+), anclada al inventario (Schmidt, 1990). *Fundamento pedagógico:* *i+1* (Krashen, 1985)
  + noticing.
- **Puerta acústica (ASR 0.70).** Bajo esa confianza de reconocimiento, el turno es **incidente**, no
  puntúa. Es la frontera que separa lo que se puede medir de lo que no.

## 3. Los tres tiers de evidencia (el eje de la propuesta)

La pronunciación y, en general, la señal de voz **no se miden todas con la misma precisión**. MLLDE lo hace
explícito con **tres tiers**; cada afirmación de voz **declara su tier**, de modo que un informe nunca afirma
más precisión que la que el motor tiene.

| Tier | Nombre | Qué mide | Cómo (fuente) | Estado |
|---|---|---|---|---|
| **1** | **Rúbrica-voz** *(medible hoy)* | `grammar_accuracy` · `vocabulary_range` · `discourse_management` · `interaction` · `global_achievement` | De la **transcripción ASR**: juez-rúbrica sobre lo dicho (texto derivado de voz). **NO pronunciación.** | **En producción** |
| **2** | **Instrumentado** *(con instrumentación)* | **Pronunciación** a nivel de palabra/enunciado: inteligibilidad y adecuación | **Evaluación de pronunciación de proveedor** (p. ej. Azure Pronunciation Assessment) — puntuación acústica tipo GOP de vendor | **Planificado** (capa acústica) |
| **3** | **GOP a medida** *(investigación)* | **Pronunciación fonémica**: rasgos objetivo por nivel, variantes aceptadas | **Inventario IPA** por nivel + **ingeniería acústica** propia (Goodness of Pronunciation; Witt & Young, 2000) | **Investigación** (contribución profunda del PhD) |

**Reglas transversales de los tiers:**
- **Honestidad de evidencia.** Un informe **declara el tier** de cada afirmación; jamás reclama la precisión
  de un tier superior al disponible. Si una destreza no tiene métrica anclada → se muestra **«—»**, no un
  valor. (Hoy: Pronunciación = «—» hasta el Tier 2; Reading/Writing no desarrollados; Listening parcial.)
- **Inteligibilidad, no acento nativo.** El objetivo es habla **inteligible y adecuada**; las **variantes
  aceptadas** (p. ej. *seseo*/*distinción*) **nunca** bajan una puntuación (IPA, 1999).
- **Ganancia incremental.** Cada tier **añade** una señal sin romper las anteriores: Tier 1 da el nivel de
  conversación hoy; Tier 2 **enciende** la banda de Pronunciación; Tier 3 la hace **fonémica y explicable**.
- **Comparabilidad.** Cada sesión declara su `measure_model`; así se pueden comparar y no mezclar sesiones de
  modelos/tiers distintos.

**Por qué tres tiers y no «todo o nada».** Un tutor comercial no puede esperar a la investigación para dar
valor; y la investigación no puede quedar cautiva de un *demo*. Los tiers permiten **lanzar con Tier 1** (voz
real, honesto) mientras se **desarrolla y valida** Tier 2 y se **investiga** Tier 3 — cada uno con su propio
diseño de validez.

## 4. Preguntas de investigación

1. **Validez.** ¿Una rúbrica CEFR aplicada por un LLM sobre transcripción ASR (Tier 1) produce bandas
   **fiables y estables** frente a la evaluación humana experta? ¿Cambia con el tamaño del modelo (p. ej.
   modelo interino pequeño vs. mayor)?
2. **Honestidad como método.** ¿La **unificación de superficies** sobre una sola verdad (LRS) funciona como
   **prueba anti-alucinación** —si todas las pantallas coinciden, el margen se sostiene?
3. **Feedback.** ¿La **escala de noticing** (dosificar la saliencia por nivel) mejora la **captación
   (*uptake*)** —auto-reparación en B2+, registro de la forma en A2–B1— sin elevar el filtro afectivo?
4. **Pronunciación por tiers.** ¿Qué gana la validez al pasar de Tier 1 → 2 → 3? ¿Cuál es el **piso de
   inteligibilidad** defendible en cada tier?

## 5. Metodología y datos

- **Diseño.** Estudio de diseño (design-based research) con un caso de aplicación end-to-end (TK Coach) +
  validación en producción.
- **Datos.** **xAPI** en un **LRS** (Veracity), **actor seudónimo**; dos flujos (medición/pedagogía);
  gate ASR 0.70; `ext/effective-time`, `ext/measure-model`, `ext/srs-schedule`, `ext/learning-target`.
- **Validez de Tier 1.** Acuerdo LLM-rúbrica vs. **evaluación humana experta** sobre una muestra; estabilidad
  test-retest; sensibilidad al modelo.
- **Auditoría de integridad.** Auditoría de medición (paneles + agentes) con matriz de hallazgos, «H0
  watchdog» (ningún descriptor pintado como banda) y verificación en producción.
- **Instrumentos de RR.HH.** Reporte por persona (alumno/profesor/RR.HH.) con marco Kirkpatrick/Phillips y
  alineación **ESCO** opcional.

## 6. Ética y cumplimiento

- **RGPD** (Reg. (UE) 2016/679): PII fuera del modelo y del LRS; seudonimización; medición en modelo de pago
  **sin entrenamiento**.
- **Ley de IA de la UE — art. 50** (Reg. (UE) 2024/1689): transparencia de contenido asistido/generado por IA;
  el chatbot se declara como IA.
- **Inteligibilidad, no acento nativo:** decisión ética y pedagógica (no penalizar variedades legítimas).

## 7. Estado y hoja de ruta

- **Tier 1 — en producción y verificado** (LRS vivo; medición interina en un modelo pequeño, declarada por
  sesión).
- **Tier 2 — planificado:** integrar evaluación de pronunciación de proveedor → encender la banda de
  Pronunciación (hoy «—»).
- **Tier 3 — investigación:** inventario IPA por nivel + GOP a medida (la contribución fonémica del PhD).
- **Transversal:** validar el *uptake* del noticing; validar la fiabilidad del scoring por tamaño de modelo.

---

## Referencias (APA 7.ª, selección)

Council of Europe. (2020). *Common European Framework of Reference for Languages: Learning, teaching,
assessment — Companion volume*. Council of Europe Publishing.

International Phonetic Association. (1999). *Handbook of the International Phonetic Association*. Cambridge
University Press.

Kirkpatrick, J. D., & Kirkpatrick, W. K. (2016). *Kirkpatrick's four levels of training evaluation*. ATD Press.

Krashen, S. D. (1985). *The input hypothesis: Issues and implications*. Longman.

Phillips, J. J., & Phillips, P. P. (2016). *Handbook of training evaluation and measurement methods* (4.ª ed.).
Routledge.

Schmidt, R. W. (1990). The role of consciousness in second language learning. *Applied Linguistics, 11*(2),
129–158. https://doi.org/10.1093/applin/11.2.129

Witt, S. M., & Young, S. J. (2000). Phone-level pronunciation scoring and assessment for interactive language
learning. *Speech Communication, 30*(2–3), 95–108. https://doi.org/10.1016/S0167-6393(99)00044-8

IEEE. (2023). *IEEE standard for learning technology — xAPI* (IEEE Std 9274.1.1-2023). IEEE SA.

Unión Europea. (2016). *Reglamento (UE) 2016/679 (RGPD)*. DOUE L 119.
Unión Europea. (2024). *Reglamento (UE) 2024/1689 (Ley de IA)*. DOUE.

---

> *© 2026 Ana Eslava-Graterol — MLLDE (UPV). TK Coach y «Capi» © Talketika. MCER © Consejo de Europa
> (parafraseado, no reproducido); Cambridge, xAPI (ADL/IEEE), IPA citados. Elaborado con asistencia de IA;
> revisado y aprobado por la autora, en el espíritu del art. 50 de la Ley de IA de la UE.*
>
> *Versión: 2026-09-05 · componente de propuesta doctoral · MLLDE + tutor por voz · 3 tiers de evidencia.*
