<!--
  Propuesta de tesis doctoral — MLLDE, tutor por voz y tres tiers de evidencia.
  Integra el documento de la autora «MLLDE y el tutor por voz: desarrollo y los tres tiers de
  evidencia» (2026-09-05) como núcleo técnico, dentro del aparato completo de una propuesta doctoral.
  © 2026 Ana Eslava-Graterol (MLLDE, UPV). TK Coach y «Capi» © Talketika.
  MCER (Consejo de Europa), xAPI (ADL/IEEE), IPA, ESCO: estándares citados, no redistribuidos.
-->

# PROPUESTA DE TESIS DOCTORAL

## MLLDE — *Multimodal Language Learning Design & Evaluation*
### Diseño curricular por modalidad para el aprendizaje móvil de lenguas y medición de la competencia oral con tres tiers de evidencia

---

| | |
|---|---|
| **Doctoranda** | Ana Zoraimy Eslava Graterol |
| **Contacto** | profeanaeslava@gmail.com · linkedin.com/in/anaeslava |
| **Programa** | Programa de Doctorado — Lingüística Aplicada |
| **Departamento** | Departamento de Lingüística Aplicada, Universitat Politècnica de València (UPV) |
| **Línea de investigación** | Tecnologías del lenguaje, evaluación de la competencia oral y diseño instruccional anclado al MCER |
| **Caso de aplicación** | TK Coach / «Capi» — tutor de inglés de negocios por voz (Talketika) |
| **Modalidad propuesta** | Tiempo parcial (4 años), compatible con actividad profesional |
| **Fecha · versión** | Septiembre de 2026 · v2.0 |

> **MLLDE** — *Multimodal Language Learning Design & Evaluation*. Método y marco de evaluación de la autora, del que esta propuesta desarrolla y valida el **Módulo de Medición**. «TK Coach» y «Capi» son marcas de Talketika; el MCER (Consejo de Europa), xAPI (ADL/IEEE), IPA y ESCO son estándares citados, no redistribuidos.

---

## 1. Resumen

Un modelo generativo es **fluido por diseño**: producirá una calificación plausible se la pidamos o no, y esa fluidez es precisamente lo que lo inhabilita como evaluador. El problema que aborda esta tesis es, por tanto, metodológico antes que técnico: **cómo convertir la producción oral real de un aprendiz frente a un agente de IA en evidencia de competencia trazable al MCER, sin que el modelo invente la nota.**

La respuesta que se propone y se valida es **MLLDE** (*Multimodal Language Learning Design & Evaluation*), un método con **dos pilares inseparables**:

- **Pilar de diseño (*Design*).** Un procedimiento replicable para construir currículo de lenguas en dispositivo móvil en el que la **modalidad** —texto, audio, imagen, **voz**— no es un envoltorio sino una **variable de diseño declarada**: cada paso de una lección especifica qué modalidad porta el insumo, la práctica y la producción, y contra qué modo y descriptor del MCER se mide.
- **Pilar de evaluación (*Evaluation*).** El **Módulo de Medición**, que convierte lo que el aprendiz produce —señaladamente su producción oral ante un agente— en evidencia trazable al MCER.

Ambos comparten la misma arquitectura, y el pilar de evaluación se articula sobre tres decisiones:

1. **Measure ≠ Decide.** El modelo **observa y describe** lo que ocurre en la interacción; un **motor determinista** —código, no IA— **computa** la banda a partir de esas observaciones. Nada de lo que aparece en pantalla ha sido inventado por un modelo.
2. **Motor + pack.** Las reglas de medición son agnósticas respecto del cliente; cada producto rellena un **pack** con sus tareas, niveles e inventario de sonidos. Aplicar el módulo a una segunda aplicación es **rellenar un pack, no rediseñar**: ahí reside la afirmación de replicabilidad que la tesis debe demostrar.
3. **Tres tiers de evidencia.** La señal de voz no se mide toda con la misma precisión. Cada afirmación **declara su tier**, de modo que un informe nunca reclame más exactitud de la que el motor realmente tiene. La pronunciación —la señal más difícil— es el caso testigo, y llevarla del Tier 1 al Tier 3 constituye la contribución fonémica profunda de la tesis.

Metodológicamente es una **investigación basada en diseño** con validación en producción: el Tier 1 ya está desplegado y emitiendo evidencia a un LRS, lo que permite contrastar el acuerdo entre la rúbrica aplicada por LLM y la **evaluación humana experta** sobre datos reales, no simulados.

**Palabras clave:** MCER · evaluación de la competencia oral · tutores por voz · GOP y pronunciación · xAPI · honestidad de la evidencia · investigación basada en diseño · lingüística aplicada.

---

## 2. Abstract *(English)*

A generative model is **fluent by design**: it will produce a plausible score whether or not it is entitled to, and that fluency is precisely what disqualifies it as an assessor. The problem this thesis addresses is therefore methodological before it is technical: **how to turn a learner's real spoken production in front of an AI agent into evidence of competence traceable to the CEFR, without the model inventing the grade.**

The proposed and validated answer is **MLLDE** (*Multimodal Language Learning Design & Evaluation*) and its **Measurement Module**, built on three design decisions:

1. **Measure ≠ Decide.** The model **observes and describes** what happens in the interaction; a **deterministic engine** — code, not AI — **computes** the band from those observations. Nothing on screen is invented by a model.
2. **Engine + pack.** The measurement rules are client-agnostic; each product fills a **pack** with its tasks, levels and sound inventory. Applying the module to a second application means **filling a pack, not redesigning**: that is the replicability claim the thesis must demonstrate.
3. **Three tiers of evidence.** Voice signal is not measurable at uniform precision. Every claim **declares its tier**, so a report never asserts more accuracy than the engine actually has. Pronunciation — the hardest signal — is the test case, and carrying it from Tier 1 to Tier 3 is the thesis's deep phonemic contribution.

Methodologically it is **design-based research with validation in production**: Tier 1 is already deployed and emitting evidence to an LRS, which allows the agreement between the LLM-applied rubric and **expert human assessment** to be tested on real rather than simulated data.

**Keywords:** CEFR · speaking assessment · voice tutors · GOP and pronunciation · xAPI · evidence honesty · design-based research · applied linguistics.

---

## 3. Justificación

**3.1 El problema de fondo: fluidez no es validez.** Los tutores conversacionales han hecho técnicamente trivial la práctica oral ilimitada. Pero un modelo de lenguaje, colocado en el papel de evaluador, no distingue entre *describir* un desempeño y *puntuarlo*: produce una banda con la misma soltura con que produce una frase. El resultado son sistemas que muestran cifras sin trazabilidad, que no soportan una auditoría y que no pueden compararse entre sí. La respuesta de MLLDE no es un mejor prompt, sino una **separación arquitectónica de responsabilidades**.

**3.2 Por qué la pronunciación es el caso decisivo.** De todas las señales que emite el habla, la pronunciación es la que más se promete en el mercado y la que menos se sostiene metodológicamente. Medirla bien exige instrumentación acústica, y afirmarla sin ella es exactamente el tipo de sobreafirmación que esta tesis quiere hacer imposible. Por eso el modelo de tiers no es un rodeo: es la manera de decir con precisión **qué se puede medir hoy, qué se puede medir con instrumentación y qué es todavía investigación**.

**3.3 Por qué tres tiers y no «todo o nada».** Un tutor comercial no puede esperar a que termine la investigación para dar valor; y la investigación no puede quedar cautiva de una demo. Los tiers permiten **lanzar con Tier 1** —voz real, medición honesta— mientras se desarrolla y valida el Tier 2 y se investiga el Tier 3, cada uno con su propio diseño de validez. Es un modelo de madurez de la evidencia, no una excusa.

**3.4 La constatación profesional.** Más de veinte años diseñando y ejecutando formación en lenguas —1.568 horas de docencia universitaria acreditadas, administración de LMS desde 2019, cursos gamificados alineados al MCER— muestran que el cuello de botella no es el contenido ni la tecnología, sino la **ausencia de un procedimiento acumulable**. MLLDE nace de ahí, y TK Coach es su primera instanciación completa.

---

## 4. Estado de la cuestión

### 4.1 El MCER como especificación de medida, no como etiqueta

El *Companion Volume* (Consejo de Europa, 2020) organiza la competencia en **modos de comunicación** —recepción, producción, interacción y **mediación**— con descriptores «can-do» por escala y nivel. En la práctica del sector, sin embargo, el MCER se usa como **etiqueta comercial** («nivel B1») y rara vez como **especificación de medida**: casi ningún producto declara, por métrica, contra qué escala nombrada se mide. MLLDE impone la regla inversa: **no hay métrica sin descriptor**, y cada métrica cita su escala y su identificador (IRI) en un *registry* único.

### 4.2 Evaluación automática del habla

La evaluación asistida por máquina de la producción oral tiene dos tradiciones que rara vez se encuentran. Por un lado, la **puntuación acústica de pronunciación**, cuyo referente sigue siendo el *Goodness of Pronunciation* (Witt & Young, 2000) y su descendencia comercial. Por otro, la **valoración holística por rúbrica**, hoy accesible a un LLM sobre transcripción. La primera es precisa y estrecha; la segunda es amplia y no verificable. **Ninguna de las dos, por sí sola, sostiene una afirmación de nivel MCER auditable.** El aporte de esta tesis es articularlas en una escala de madurez explícita —los tres tiers— en lugar de elegir una y ocultar sus límites.

### 4.3 Retroalimentación, *noticing* e *i+1*

La hipótesis del insumo comprensible (Krashen, 1985) y la hipótesis del *noticing* (Schmidt, 1990) fundamentan que la retroalimentación sea **dosificada por nivel** y no uniforme. MLLDE lo operacionaliza como una **escala de noticing (0–4)** que gradúa la saliencia dentro del *recast*: **modelar** en A2–B1, **elicitar** en B2+. Lo relevante metodológicamente es quién decide qué: **el código decide el nivel de feedback (0–3); el LLM detecta y redacta.**

### 4.4 Inteligibilidad frente a acento nativo

La literatura sobre inteligibilidad y la propia posición de la IPA (1999) sostienen que el objetivo defendible es el **habla inteligible y adecuada**, no la aproximación a un acento nativo. MLLDE lo convierte en regla del motor: las **variantes aceptadas** (por ejemplo *seseo* / *distinción*) **nunca** rebajan una puntuación. Es una decisión ética además de técnica, y tiene consecuencias directas sobre el diseño del inventario fonémico del Tier 3.

### 4.5 Datos de aprendizaje interoperables

xAPI (IEEE Std 9274.1.1-2023) y los LRS permiten registrar experiencias fuera del LMS. Lo que no existe es un **perfil consolidado y abierto para evidencia de competencia lingüística anclada a descriptores del MCER**, con declaración explícita del modelo de medición y del tier de cada afirmación. Sin eso, dos plataformas no son comparables aunque ambas digan «B1».

### 4.6 El vacío

> No existe un **método replicable y auditable** que (a) separe explícitamente **observación de decisión** en la evaluación de la producción oral asistida por IA, (b) ancle cada métrica a una escala nombrada del MCER, (c) **declare el grado de precisión** de cada afirmación mediante un modelo de tiers, y (d) emita esa evidencia en un formato interoperable que permita comparar sesiones, modelos y productos. Esta tesis lo construye y lo somete a prueba sobre un sistema en producción.

---

## 5. El método: MLLDE y su Módulo de Medición

### 5.1 Principios

| Principio | Qué significa operativamente |
|---|---|
| **Measure ≠ Decide** | El LLM describe; un motor determinista computa la banda. Ninguna cifra procede de una generación. |
| **No hay métrica sin descriptor** | Cada métrica cita una escala nombrada del *Companion Volume* y su IRI en un registry único. |
| **Motor + pack** | Reglas agnósticas del cliente; cada producto aporta tareas, niveles e inventario de sonidos. |
| **Cinco destrezas** | Recepción, producción, interacción y **mediación**, todas ancladas al *Companion Volume*. |
| **Trazabilidad** | Toda la evidencia se registra en **xAPI** sobre un LRS, con actor seudónimo. |
| **Honestidad de la evidencia** | Cada afirmación declara su **tier** y su **modelo de medición** por sesión. |

**Escala.** 0–10 (aprobado ≥ 6, pisos ≥ 4), con vista Cambridge 0–5 por redondeo y división entre 2.

### 5.2 El pilar de diseño: la modalidad como variable declarada

El mismo principio que gobierna la medición gobierna el diseño: **nada implícito**. Si la medición exige que toda métrica cite su descriptor, el diseño exige que **todo paso de una lección declare su modalidad y su modo del MCER**.

**Contrato de entrada de una lección.** Nivel MCER + descriptor «can-do» + escenario real + **perfil de modalidad**. Ese cuarto elemento es la aportación del pilar de diseño: el perfil declara, paso a paso, qué canal porta el insumo, cuál soporta la práctica y en cuál se exige la producción.

| Paso de la lección | Modo del MCER | Modalidad del insumo | Modalidad de la producción |
|---|---|---|---|
| Llegada — gancho y objetivo | — | texto + imagen | — |
| Vocabulario y *chunks* | Recepción | audio + imagen (codificación dual) | reconocimiento |
| Diálogo modelo | Recepción | **voz** | — |
| Práctica guiada | Procesamiento | texto o audio | texto |
| Misión — tarea auténtica | **Interacción** | **voz** (agente) | **voz** |
| Transferencia | Producción | libre | **voz o escritura, a elección** |
| Cultura y pragmática | — | texto + imagen | — |

**Por qué importa para una tesis y no solo para un producto.** La literatura de aprendizaje móvil describe *principios* (brevedad, contexto, microaprendizaje) pero rara vez un **procedimiento** que otro equipo pueda reproducir, y casi nunca trata la modalidad como algo que se decide y se justifica. Declararla tiene tres consecuencias comprobables: hace la lección **auditable** (se puede verificar que el modo del MCER y el canal coinciden), **replicable** (dos diseñadoras que parten del mismo descriptor y el mismo perfil deberían producir lecciones equivalentes) y **medible** (la evidencia que emite cada paso ya sabe a qué modo pertenece).

**Motor + pack, también en el diseño.** El ciclo de la lección es un **motor** compartido; una lección concreta es un **objeto de datos**. Construir una lección nueva —o una lengua nueva— es **rellenar datos, no reescribir lógica**. Es la misma promesa de replicabilidad que sostiene el pilar de evaluación, y se somete a la misma prueba (PI6).

**Marcos que sintetiza el pilar de diseño**, todos acreditados y ninguno inventado: el ciclo gamificado **IPO** (Casañ-Pitarch, 2017); las **4C del AICLE** (Coyle, 2007); **ESA** (Harmer, 2007); **CTL / REACT** (Johnson, 2002; Crawford, 2001) para la autenticidad de la tarea; el **enfoque léxico** (Lewis, 1993) para la enseñanza por *chunks*; y la **teoría cognitiva del aprendizaje multimedia** (Mayer, 2009), que es justamente la que fundamenta tratar la modalidad como decisión y no como adorno. La originalidad no está en ninguno de ellos, sino en **la síntesis operacionalizada y en la declaración explícita de modalidad**.

### 5.3 Arquitectura del tutor por voz

El aprendiz practica **hablando** situaciones reales de trabajo con «Capi». El bucle de medición es:

> **Capi (role-play)** → **Evaluador MLLDE** (banda 0–10 + descriptor débil *i+1*) → **Práctica** (drills, tarjetas, mediación) → **Capi** → la banda sube **en la conversación siguiente**.

- **Tres agentes que observan** (Capi · corrector · evaluador) y un **consolidador escrito en código** —no un cuarto LLM— que computa el nivel acumulativo (`Global×5 + analíticas×2 ÷ pool × 10`) y emite **una sola entrada** al LRS. Un **redactor** escribe el resumen; no mide. Los **generadores** crean contenido: el código elige el descriptor, el LLM lo redacta.
- **Dos flujos que nunca se cruzan:** *medición* (una vez por sesión: `completed` + rúbrica) y *pedagogía* (por turno: `adapted` + `pedagogical-action` + `learning-target`). **La corrección es pedagogía y nunca puntúa** — es el cortafuegos que hace auditable el sistema.
- **Puerta acústica (ASR 0.70).** Por debajo de esa confianza de reconocimiento el turno se registra como **incidente** y no puntúa. Es la frontera explícita entre lo medible y lo no medible.

### 5.4 Los tres tiers de evidencia

| Tier | Nombre | Qué mide | Cómo | Estado |
|---|---|---|---|---|
| **1** | **Rúbrica-voz** *(medible hoy)* | `grammar_accuracy` · `vocabulary_range` · `discourse_management` · `interaction` · `global_achievement` | Juez-rúbrica sobre la **transcripción ASR**. **No mide pronunciación.** | **En producción**, verificado sobre LRS vivo |
| **2** | **Instrumentado** | **Pronunciación** a nivel de palabra y enunciado: inteligibilidad y adecuación | Evaluación de pronunciación de proveedor (puntuación acústica tipo GOP) | **Planificado** — capa acústica |
| **3** | **GOP a medida** *(investigación)* | **Pronunciación fonémica**: rasgos objetivo por nivel, variantes aceptadas | **Inventario IPA** por nivel + ingeniería acústica propia (Witt & Young, 2000) | **Investigación** — contribución profunda de la tesis |

**Reglas transversales.** *(i)* Un informe **declara el tier** de cada afirmación y jamás reclama la precisión de un tier superior; si una destreza carece de métrica anclada se muestra **«—»**, nunca un valor (hoy: pronunciación = «—» hasta el Tier 2). *(ii)* **Inteligibilidad, no acento nativo**: las variantes aceptadas no bajan puntuación. *(iii)* **Ganancia incremental**: cada tier añade señal sin romper los anteriores. *(iv)* **Comparabilidad**: cada sesión declara su `measure_model`, de modo que no se mezclen sesiones de tiers o modelos distintos.

---

## 6. Preguntas de investigación, objetivos e hipótesis

### 6.1 Preguntas

| # | Pregunta | Ciclo |
|---|---|---|
| **PI1 · Validez** | ¿Una rúbrica MCER aplicada por un LLM sobre transcripción ASR (Tier 1) produce bandas **fiables y estables** frente a la evaluación humana experta? ¿Varía con el tamaño del modelo? | C1 |
| **PI2 · Honestidad como método** | ¿Funciona la **unificación de superficies sobre una sola verdad** (el LRS) como prueba anti-alucinación? Es decir: si todas las pantallas coinciden, ¿se sostiene el margen? | C1–C2 |
| **PI3 · Retroalimentación** | ¿La **escala de noticing** —dosificar la saliencia según el nivel— mejora la **captación (*uptake*)** (auto-reparación en B2+, registro de la forma en A2–B1) sin elevar el filtro afectivo? | C2 |
| **PI4 · Pronunciación por tiers** | ¿Qué gana la validez al pasar de Tier 1 → 2 → 3? ¿Cuál es el **piso de inteligibilidad** defendible en cada tier? | C2–C3 |
| **PI5 · Diseño por modalidad** | ¿Produce el **perfil de modalidad declarado** lecciones equivalentes entre diseñadoras distintas que parten del mismo descriptor? ¿Y afecta la elección de modalidad a la progresión en el modo del MCER que se pretende desarrollar? | C1–C2 |
| **PI6 · Replicabilidad** | ¿Puede un equipo independiente instanciar **el motor de diseño y el de medición** en una segunda aplicación **rellenando un pack**, sin tocar el motor, y obtener lecciones y medidas comparables? | C3 |

### 6.2 Objetivos

1. **O1** — Formalizar el Módulo de Medición MLLDE (principios, registry de escalas, esquema de packs, reglas del consolidador) en una especificación verificable por terceros.
2. **O2** — Establecer la **validez del Tier 1**: acuerdo con evaluación humana experta, estabilidad test-retest y sensibilidad al tamaño del modelo.
3. **O3** — Instrumentar y validar el **Tier 2**, encendiendo la banda de pronunciación hoy declarada «—», y determinar su piso de inteligibilidad.
4. **O4** — Desarrollar el **Tier 3**: inventario IPA por nivel con variantes aceptadas y un GOP a medida, explicable y no penalizador de variedades legítimas.
5. **O5** — Formalizar el **pilar de diseño**: contrato de entrada con perfil de modalidad, plantilla de planificación, rúbrica de conformidad, y validarlo mediante panel de personas expertas y prueba de equivalencia entre diseñadoras.
6. **O6** — Publicar el **perfil xAPI** de evidencia de competencia anclada al MCER, con declaración de tier y de modelo de medición, y demostrar la **replicabilidad motor + pack** —diseño y medición— en una segunda aplicación.

### 6.3 Hipótesis

| # | Hipótesis | Contraste |
|---|---|---|
| **H1** | El acuerdo entre la banda del Tier 1 y la evaluación humana experta alcanza una fiabilidad aceptable para uso formativo, y es **estable** en test-retest. | CCI / κ ponderado; test-retest |
| **H2** | La banda del Tier 1 es **sensible al tamaño del modelo**, lo que obliga a declarar `measure_model` para que las sesiones sean comparables. | Comparación entre modelos sobre las mismas sesiones |
| **H3** | La escala de noticing dosificada por nivel aumenta el ***uptake*** frente a una retroalimentación uniforme, sin aumentar el abandono. | Contraste entre condiciones + métricas de persistencia |
| **H4** | El paso a Tier 2 mejora la validez de la afirmación de pronunciación frente a juicio humano de inteligibilidad; el Tier 3 la hace además **explicable** a nivel fonémico. | Validez concurrente por tier |
| **H5** | Diseñadoras distintas que parten del mismo descriptor y perfil de modalidad producen lecciones con **alta concordancia** en modo, competencia y canal. | Acuerdo interjueces sobre rúbrica de conformidad |
| **H6** | Un equipo independiente reproduce **lecciones y medidas** comparables **rellenando un pack**, sin modificar el motor. | Prueba de replicabilidad end-to-end |

---

## 7. Metodología

### 7.1 Diseño

**Investigación basada en diseño (DBR) con validación en producción.** El objeto es a la vez un artefacto (el módulo) y un conocimiento (los principios que lo sostienen). Que el Tier 1 esté **ya desplegado** distingue esta propuesta de un estudio de laboratorio: los datos de validez proceden de uso real, no de simulaciones.

| Ciclo | Foco | Objetivos | Métodos |
|---|---|---|---|
| **C1 — Formalización y validez del Tier 1** | El método y la medida que ya existe | O1, O2, O5 | Formalización de ambos pilares; **panel Delphi** sobre el contrato de diseño; **prueba de equivalencia** con diseñadoras independientes; muestreo de sesiones del LRS; **doble evaluación humana experta** con acuerdo interjueces; test-retest; sensibilidad al modelo; auditoría de integridad |
| **C2 — Instrumentación y feedback** | Pronunciación Tier 2 + noticing | O3 | Integración de la capa acústica; validez concurrente frente a juicio de inteligibilidad; estudio del *uptake* con condiciones de saliencia contrastadas; *think-aloud* |
| **C3 — Tier 3 y replicabilidad** | La contribución fonémica y la prueba del método | O4, O6 | Inventario IPA por nivel; GOP a medida; validación fonémica; **prueba de replicabilidad end-to-end** (diseño + medición) con equipo independiente rellenando un pack; publicación del perfil xAPI |

### 7.2 Datos e instrumentos

- **Evidencia de aprendizaje:** sentencias **xAPI** en un **LRS** (Veracity), **actor seudónimo**, dos flujos separados (medición / pedagogía), puerta ASR 0.70, y las extensiones `ext/effective-time`, `ext/measure-model`, `ext/srs-schedule`, `ext/learning-target`.
- **Criterio humano:** panel de evaluadores expertos con formación MCER, doble corrección ciega sobre una submuestra y acuerdo reportado.
- **Pronunciación:** juicios humanos de inteligibilidad como criterio externo para los Tiers 2 y 3.
- **Auditoría de integridad:** auditoría de medición con matriz de hallazgos, un ***«H0 watchdog»*** que verifica que **ningún descriptor se pinte como si fuera una banda**, y verificación en producción.
- **Instrumentos de transferencia:** informes por persona (aprendiz / docente / RR. HH.) bajo marco Kirkpatrick y Phillips, con alineación **ESCO** opcional.

### 7.3 Análisis

Fiabilidad interjueces (CCI, κ ponderado) y acuerdo LLM–humano; estabilidad test-retest; modelos mixtos para el efecto de la condición de saliencia sobre el *uptake*, con el centro como efecto aleatorio; validez concurrente por tier con intervalos de confianza; análisis de secuencias sobre xAPI para reconstruir trayectorias reales; análisis temático de los *think-aloud*. **Preinscripción** del plan analítico de cada ciclo antes de la recogida.

### 7.4 Ética y cumplimiento

1. **RGPD** (Reg. UE 2016/679): datos personales fuera del modelo y del LRS; seudonimización en origen; medición sobre servicio de pago **sin entrenamiento** con los datos.
2. **Ley de IA de la UE, art. 50** (Reg. UE 2024/1689): el agente se declara como IA ante el aprendiz; el contenido asistido o generado se etiqueta.
3. **Inteligibilidad, no acento nativo:** decisión ética explícita — no penalizar variedades legítimas del inglés.
4. **Comité de ética** de la UPV antes del ciclo 2. Participación voluntaria y revocable; personas menores excluidas.
5. **Accesibilidad:** WCAG 2.1 AA en todas las superficies de la intervención.
6. **Propiedad intelectual:** el MCER se parafrasea y se cita, no se reproduce; Cambridge, xAPI (ADL/IEEE), IPA y ESCO se citan como estándares.

### 7.5 Limitaciones previstas

Dependencia de proveedores comerciales de ASR y de evaluación de pronunciación (mitigada declarando `measure_model` por sesión y anclando el contrato al método, no al proveedor); el caso testigo es **inglés de negocios**, de modo que la generalización a otras lenguas y dominios se apoya en la prueba de packs y debe reportarse como límite de alcance; autoselección de las personas usuarias de un producto en producción; posible efecto de novedad, mitigado con medidas de seguimiento.

---

## 8. Plan de trabajo

Modalidad a **tiempo parcial, cuatro años**.

| Año | Hitos | Entregable |
|---|---|---|
| **1** | Revisión sistemática; especificación formal del Módulo de Medición y del registry de escalas; diseño del estudio de validez del Tier 1; solicitud al comité de ética; convenios | Especificación v1.0 · plan de investigación aprobado |
| **2** | Ciclo 1 completo: muestreo del LRS, doble evaluación humana experta, test-retest, sensibilidad al modelo, auditoría de integridad | **Artículo 1** — validez del Tier 1 · perfil xAPI v0.9 |
| **3** | Ciclo 2: integración de la capa acústica (Tier 2), validez concurrente, estudio del *uptake* del noticing; estancia de investigación | **Artículo 2** — pronunciación instrumentada y noticing |
| **4** | Ciclo 3: inventario IPA y GOP a medida (Tier 3); prueba de replicabilidad motor + pack; redacción, depósito y defensa | **Artículo 3** — GOP fonémico · tesis depositada · mención internacional |

**Mención internacional:** estancia de tres meses en el año 3 en un grupo europeo de referencia en evaluación del habla o CALL, y redacción de parte de la tesis en inglés.

---

## 9. Resultados esperados y contribución original

1. **Una especificación abierta de MLLDE en sus dos pilares** — el contrato de diseño con perfil de modalidad y su rúbrica de conformidad, y el Módulo de Medición con su registry de escalas MCER, esquema de packs y reglas del consolidador, aplicables por terceros.
2. **Evidencia de validez del Tier 1** — acuerdo con evaluación humana experta, estabilidad y sensibilidad al modelo, sobre datos de producción.
3. **La pronunciación, encendida y explicada** — del «—» honesto al Tier 2 instrumentado y al Tier 3 fonémico, con inventario IPA por nivel y variantes aceptadas.
4. **Un perfil xAPI abierto** para evidencia de competencia anclada al MCER, con declaración de tier y de modelo de medición.
5. **La prueba de replicabilidad motor + pack** en una segunda aplicación.
6. **Una política de honestidad de la evidencia** transferible a cualquier producto educativo con IA.

**Originalidad.** No está en proponer una rúbrica nueva ni un algoritmo acústico nuevo, sino en **una arquitectura de responsabilidad**: separar observación de decisión, obligar a cada afirmación a declarar su grado de precisión, y hacer ambas cosas verificables en datos interoperables. Es una aportación metodológica a la evaluación asistida por IA, con la pronunciación como caso testigo llevado hasta el nivel fonémico.

---

## 10. Difusión

**Revistas objetivo:** *Language Testing* · *Assessing Writing / Assessing Speaking* · *ReCALL* · *Computer Assisted Language Learning* · *Language Learning & Technology* · *Speech Communication* · *System* · *Computers & Education* · *RESLA* · *Educación XX1*.

**Congresos:** EUROCALL · WorldCALL · Interspeech / SLaTE · ALTE · EALTA · AESLA · AELFE · Jornadas de Innovación Educativa y Docencia en Red (UPV).

**Acceso abierto:** especificación, registry, rúbricas y perfil xAPI en repositorio público; RiuNet (UPV); ORCID.

---

## 11. Viabilidad y encaje

**Técnica.** El Tier 1 está **en producción y verificado** sobre un LRS vivo; la doctoranda administra LMS desde 2019, empaqueta SCORM/xAPI y ha construido el sistema completo. La infraestructura de recogida existe: no hay que crearla, hay que validarla.

**Acceso al campo.** Población real de aprendices adultos a través de TK Coach, más veinte años de docencia y la acreditación como examinadora DELE del Instituto Cervantes.

**Recursos.** LRS (Veracity, ya operativo); créditos de API de LLM y de evaluación de pronunciación de proveedor para el Tier 2; tiempo de evaluadores humanos expertos (partida principal); herramientas estadísticas abiertas; financiación para estancia y publicación en acceso abierto — se concurrirá a convocatorias predoctorales y de movilidad.

**Encaje con la UPV.** La propuesta se inscribe en el **Departamento de Lingüística Aplicada**, donde la doctoranda cursó el máster y desarrolló su investigación de corpus sobre metadiscurso, y donde el modelo IPO gamificado que alimenta el diseño instruccional de MLLDE fue desarrollado.

---

## 12. Referencias (APA 7.ª)

Advanced Distributed Learning Initiative. (2017). *xAPI profiles specification* (Version 1.0). https://adlnet.github.io/xapi-profiles/

Casañ-Pitarch, R. (2017). *An approach to digital game-based learning: Video-games principles for language learning*. Journal of Language Teaching and Research.

Council of Europe. (2020). *Common European Framework of Reference for Languages: Learning, teaching, assessment — Companion volume*. Council of Europe Publishing.

Coyle, D. (2007). Content and language integrated learning: Towards a connected research agenda for CLIL pedagogies. *International Journal of Bilingual Education and Bilingualism, 10*(5), 543–562.

Crawford, M. L. (2001). *Teaching contextually: Research, rationale, and techniques for improving student motivation and achievement in mathematics and science*. CCI Publishing / CORD.

European Commission. (n.d.). *ESCO: European Skills, Competences, Qualifications and Occupations*. Recuperado el 5 de septiembre de 2026, de https://esco.ec.europa.eu/

IEEE. (2023). *IEEE standard for learning technology — JSON data model format and RESTful web service for learner experience data tracking and access (xAPI)* (IEEE Std 9274.1.1-2023). IEEE Standards Association.

International Phonetic Association. (1999). *Handbook of the International Phonetic Association: A guide to the use of the International Phonetic Alphabet*. Cambridge University Press.

Harmer, J. (2007). *The practice of English language teaching* (4.ª ed.). Pearson Longman.

Johnson, E. B. (2002). *Contextual teaching and learning: What it is and why it's here to stay*. Corwin Press.

Kirkpatrick, J. D., & Kirkpatrick, W. K. (2016). *Kirkpatrick's four levels of training evaluation*. ATD Press.

Krashen, S. D. (1985). *The input hypothesis: Issues and implications*. Longman.

Lewis, M. (1993). *The lexical approach: The state of ELT and a way forward*. Language Teaching Publications.

Mayer, R. E. (2009). *Multimedia learning* (2.ª ed.). Cambridge University Press.

Phillips, J. J., & Phillips, P. P. (2016). *Handbook of training evaluation and measurement methods* (4.ª ed.). Routledge.

Schmidt, R. W. (1990). The role of consciousness in second language learning. *Applied Linguistics, 11*(2), 129–158. https://doi.org/10.1093/applin/11.2.129

Unión Europea. (2016). *Reglamento (UE) 2016/679, General de Protección de Datos*. DOUE L 119.

Unión Europea. (2024). *Reglamento (UE) 2024/1689, Ley de Inteligencia Artificial*. DOUE.

Witt, S. M., & Young, S. J. (2000). Phone-level pronunciation scoring and assessment for interactive language learning. *Speech Communication, 30*(2–3), 95–108. https://doi.org/10.1016/S0167-6393(99)00044-8

> **Nota.** Antes del depósito conviene ampliar §4.2 con la literatura 2024–2026 sobre evaluación automática del habla con modelos de lenguaje, y §4.3 con los trabajos recientes sobre *uptake* y retroalimentación correctiva en interacción con agentes.

---

*© 2026 Ana Eslava-Graterol — MLLDE (Universitat Politècnica de València). TK Coach y «Capi» © Talketika. El MCER (Consejo de Europa) se parafrasea y se cita, no se reproduce; Cambridge, xAPI (ADL/IEEE), IPA y ESCO se citan como estándares. Elaborado con asistencia de IA; revisado y aprobado por la autora, en el espíritu del art. 50 de la Ley de IA de la UE.*
