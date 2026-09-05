<!--
  Propuesta de tesis doctoral — MLLDE.
  © 2026 Ana Eslava-Graterol (ProfeAnaEslavaEdTech). Todos los derechos reservados.
  "Language Passport"™ y "Grace" son marcas de la autora. MLLDE es la metodología subyacente.
  MCER/CEFR (Consejo de Europa), Plan curricular (Instituto Cervantes), xAPI (ADL/IEEE),
  ESCO (Unión Europea) e IPA son estándares citados, no redistribuidos.
-->

# PROPUESTA DE TESIS DOCTORAL

## MLLDE — *Mobile Language Learning Design Environment*
### Método para integrar tutores LLM y literacidad en IA en el diseño curricular CEFR

---

| | |
|---|---|
| **Doctoranda** | Ana Zoraida Eslava-Graterol |
| **Contacto** | profeanaeslava@gmail.com · https://www.linkedin.com/in/anaeslava |
| **Programa** | Programa de Doctorado — Lingüística Aplicada |
| **Departamento** | Departamento de Lingüística Aplicada, Universitat Politècnica de València (UPV) |
| **Línea de investigación** | Tecnologías del lenguaje, diseño instruccional y aprendizaje de lenguas asistido por dispositivos móviles |
| **Modalidad propuesta** | Tiempo parcial (4 años), compatible con actividad profesional |
| **Fecha** | Septiembre de 2026 |
| **Versión** | 1.0 |

> *Esta propuesta desarrolla y somete a validación empírica el método MLLDE, del que la autora es titular. «Language Passport»™ y «Grace» son marcas de la autora; MLLDE es la metodología subyacente. El MCER (Consejo de Europa), el Plan curricular del Instituto Cervantes, xAPI (ADL/IEEE), ESCO (Unión Europea) e IPA son estándares citados, no redistribuidos.*

---

## 1. Resumen

El aprendizaje de lenguas asistido por dispositivos móviles (MALL) y los tutores conversacionales basados en grandes modelos de lenguaje (LLM) se han popularizado con enorme rapidez, pero su incorporación al aula y al currículo sigue siendo **artesanal, no replicable y difícilmente evaluable**. Faltan tres cosas a la vez: (i) un **procedimiento de diseño** que convierta un descriptor «can-do» del MCER en una lección móvil jugable de forma sistemática; (ii) un tratamiento de la **literacidad en IA generativa** como *objetivo curricular explícito* del aprendiz de lenguas, y no como un efecto colateral del uso de la herramienta; y (iii) una **arquitectura de datos de aprendizaje interoperable** (xAPI/cmi5) que ancle cada evidencia de desempeño a un descriptor del MCER y permita comparar resultados entre lenguas, instituciones y plataformas.

Esta tesis propone, formaliza y valida empíricamente el **MLLDE (*Mobile Language Learning Design Environment*)**: un método de diseño replicable, agnóstico respecto de la lengua, que articula el ciclo IPO gamificado (Casañ-Pitarch, 2017), las 4C del AICLE (Coyle, 2007), el aprendizaje contextual CTL/REACT (Johnson, 2002; Crawford, 2001), el enfoque léxico (Lewis, 1993) y los principios de diseño para móvil (Clothier, 2026), **anclados en su totalidad a los modos y competencias del MCER** (Consejo de Europa, 2020) y, para el español, al *Plan curricular del Instituto Cervantes*. Sobre ese armazón, el método incorpora dos elementos nuevos: un **tutor LLM con función pedagógica delimitada** dentro de una escalera de retroalimentación no punitiva, y un **módulo de literacidad en IA** integrado en la propia secuencia de la lección.

La investigación se articula como **investigación basada en diseño (DBR)** en tres macrociclos iterativos, con metodología mixta: validación del método por panel de personas expertas (Delphi), intervención con aprendices adultos de lengua en niveles A2–B2, y medición de resultados en tres planos — progresión en descriptores MCER, competencia en IA generativa y autoeficacia. Los resultados esperados son un método formalizado y validado, una especificación abierta de perfil xAPI para datos de aprendizaje de lenguas anclados al MCER, y evidencia empírica sobre el efecto de la tutoría LLM pedagógicamente delimitada frente a su uso no estructurado.

**Palabras clave:** MCER · MALL · tutores LLM · literacidad en IA · diseño instruccional · investigación basada en diseño · xAPI · AICLE · gamificación · aprendizaje de lenguas.

---

## 2. Abstract *(English)*

Mobile-assisted language learning (MALL) and conversational tutors built on large language models (LLMs) have spread with remarkable speed, yet their incorporation into classrooms and curricula remains **craft-based, non-replicable and hard to evaluate**. Three things are missing at once: (i) a **design procedure** that systematically turns a CEFR can-do descriptor into a playable mobile lesson; (ii) a treatment of **generative-AI literacy** as an *explicit curricular objective* for the language learner rather than a by-product of tool use; and (iii) an **interoperable learning-data architecture** (xAPI/cmi5) that anchors every performance evidence to a CEFR descriptor and makes results comparable across languages, institutions and platforms.

This thesis proposes, formalises and empirically validates **MLLDE (Mobile Language Learning Design Environment)**: a replicable, language-agnostic design method that articulates the gamified IPO cycle (Casañ-Pitarch, 2017), the CLIL 4Cs (Coyle, 2007), contextual teaching and learning (Johnson, 2002; Crawford, 2001), the lexical approach (Lewis, 1993) and mobile learning design principles (Clothier, 2026), **anchored throughout to the CEFR modes and competences** (Council of Europe, 2020) and, for Spanish, to the *Plan curricular del Instituto Cervantes*. On that scaffold the method adds two new elements: an **LLM tutor with a bounded pedagogical role** inside a non-punitive feedback ladder, and an **AI-literacy module** embedded in the lesson sequence itself.

The research is designed as **design-based research (DBR)** across three iterative macro-cycles, using mixed methods: expert-panel validation of the method (Delphi), an intervention with adult language learners at A2–B2, and outcome measurement on three planes — CEFR descriptor progression, generative-AI competence, and self-efficacy. Expected outputs are a formalised, validated method, an open xAPI profile specification for CEFR-anchored language-learning data, and empirical evidence on the effect of pedagogically bounded LLM tutoring versus unstructured use.

**Keywords:** CEFR · MALL · LLM tutors · AI literacy · instructional design · design-based research · xAPI · CLIL · gamification · language learning.

---

## 3. Justificación y motivación

Tres constataciones, una profesional y dos académicas, motivan esta propuesta.

**3.1 La constatación profesional.** A lo largo de más de veinte años diseñando y ejecutando formación en lenguas — 1.568 horas acreditadas de docencia universitaria, la administración de un LMS desde 2019 y el diseño íntegro de cursos gamificados alineados al MCER — el problema recurrente no ha sido la falta de contenido ni la falta de tecnología, sino la **falta de un procedimiento**. Cada curso se rediseña desde cero; cada docente reinventa la secuencia; el conocimiento de diseño no se acumula. El proyecto *Academic Writing Journey* (calificado 10/10 por diseño inclusivo, UPV, 2026) mostró que un ciclo pedagógico explícito y documentado sí es reutilizable — y ésa es la semilla de MLLDE.

**3.2 La constatación sobre los tutores LLM.** Los modelos de lenguaje han hecho técnicamente trivial lo que antes era caro: una interacción conversacional ilimitada, con corrección inmediata, en la lengua meta. Pero *conversar con un modelo* no es *aprender una lengua*. Sin un contrato pedagógico explícito, el tutor LLM tiende a (a) resolver la tarea en lugar de andamiarla, (b) producir un insumo lingüístico no calibrado al nivel del aprendiz, rompiendo la condición de *i+1* (Krashen, 1985), y (c) desplazar la evaluación auténtica hacia una interacción sin evidencia registrable. La pregunta relevante ya no es *si* usar un tutor LLM, sino **con qué límites, en qué paso del ciclo de aprendizaje y bajo qué registro de evidencia**.

**3.3 La constatación sobre la literacidad en IA.** El estudio de Carnegie Mellon sobre competencia en IA generativa identifica cuatro competencias medibles —conocimiento del funcionamiento de los LLM, habilidad de *prompting*, verificación de hechos y fuentes, y autoeficacia— y muestra que una intervención breve, asíncrona, con práctica activa y retroalimentación explicativa produce mejoras significativas y equitativas entre grupos demográficos. Sin embargo, esa literacidad se enseña hoy en cursos aparte, desconectados del contenido. En una clase de lenguas, donde el aprendiz **ya está usando** el modelo como interlocutor, existe una oportunidad singular: enseñar a evaluar críticamente la producción del modelo **es, a la vez**, una tarea de recepción, de mediación y de competencia pragmática en la lengua meta. La literacidad en IA no compite con el currículo de lenguas: se puede **anclar en él**.

**3.4 El marco normativo.** El Reglamento Europeo de Inteligencia Artificial, y en particular sus obligaciones de transparencia (art. 50), junto con el RGPD y el Acta Europea de Accesibilidad, convierten la trazabilidad y la divulgación del contenido generado por IA en un requisito de diseño, no en una consideración posterior. Un método de diseño publicado hoy debe incorporar esa capa desde el origen. MLLDE lo hace.

---

## 4. Estado de la cuestión

### 4.1 El MCER como núcleo de competencia, no como etiqueta de nivel

El Marco Común Europeo de Referencia (Consejo de Europa, 2020) sustituye las cuatro destrezas tradicionales por **cuatro modos de comunicación** —recepción, producción, interacción y mediación— sostenidos por **tres competencias comunicativas** —lingüística, sociolingüística y pragmática—, y describe el progreso mediante descriptores «can-do» en seis niveles (A1–C2). En la práctica del sector, sin embargo, el MCER se usa mayoritariamente como **etiqueta comercial de nivel** («curso B1») y no como **especificación de diseño**. Muy pocos productos declaran, por tarea, qué modo y qué competencia desarrollan y contra qué descriptor se mide el resultado. Ese uso débil del estándar es la causa directa de la incomparabilidad de resultados entre plataformas.

### 4.2 MALL: eficacia demostrada, diseño poco documentado

La literatura sobre aprendizaje móvil de lenguas acredita ventajas de accesibilidad, microaprendizaje y práctica distribuida, y Clothier (2026) sistematiza los principios de diseño para móvil: diseño dirigido por el contexto, brevedad y escaneabilidad, empatía con el aprendiz, con microlearning, narrativa, gamificación y apoyo al desempeño como estrategias. Lo que la literatura documenta con menos frecuencia es **el procedimiento**: cómo se pasa de un objetivo curricular a una lección móvil concreta de manera que otro equipo pueda reproducirla. Sin ese eslabón, la evidencia sobre eficacia no es transferible.

### 4.3 Gamificación e integración de contenido y lengua

El modelo IPO (*Input–Processing–Output*) de Casañ-Pitarch (2017) aporta un ciclo de aprendizaje gamificado con arquitectura de anillos y una identidad narrativa disciplinar; las 4C de Coyle (2007, 2010) —contenido, comunicación, cognición y cultura— aportan la integración; ESA (Harmer, 2007) aporta la puesta en escena (*Engage–Study–Activate*); CTL y las estrategias REACT (Johnson, 2002; Crawford, 2001) aportan la autenticidad de la tarea y la transferencia; el enfoque léxico (Lewis, 1993) aporta la enseñanza por *chunks*; la teoría cognitiva del aprendizaje multimedia (Mayer, 2009) aporta la codificación dual del vocabulario; y la pragmática interlingüística (Kasper & Rose, 2001) aporta el tratamiento explícito del registro y la cortesía. **Existen todas las piezas; no existe la síntesis operacionalizada.** MLLDE es esa síntesis, y su originalidad reside en el ensamblaje replicable, no en la invención de un marco nuevo.

### 4.4 Tutores LLM en aprendizaje de lenguas

La investigación reciente sobre tutores conversacionales basados en LLM se ha centrado en la calidad de la corrección, la percepción del aprendiz y la reducción de la ansiedad comunicativa. Persisten tres vacíos: **la calibración del insumo** al nivel MCER del aprendiz, **la delimitación funcional** del tutor dentro de la secuencia didáctica (¿corrige?, ¿explica?, ¿evalúa?, ¿sustituye a la tarea?), y **la registrabilidad** de la interacción como evidencia de aprendizaje. MLLDE aborda los tres mediante una **escalera de retroalimentación** en la que el modelo sólo interviene en el último escalón, después de las reglas deterministas y de la gramática de referencia enlazada.

### 4.5 Literacidad en IA generativa

El estudio de Carnegie Mellon define un constructo medible en cuatro competencias y valida un diseño de intervención —módulos asíncronos, aprender haciendo, retroalimentación explicativa inmediata— con resultados significativos y equitativos. Trasladado a la enseñanza de lenguas, ese constructo es **enseñable dentro de la propia tarea comunicativa**, no fuera de ella: verificar la salida del modelo es una tarea de recepción crítica; reformular una instrucción es una tarea de producción; explicar a otra persona por qué la respuesta del modelo era inadecuada es, en términos del MCER, **mediación** — el modo que el propio marco sitúa en los niveles B2 y superiores.

### 4.6 Datos de aprendizaje interoperables

xAPI (ADL, 2017; IEEE 9274.1.1-2023) y cmi5 permiten registrar experiencias de aprendizaje fuera del LMS y almacenarlas en un LRS. Los perfiles xAPI publicados cubren dominios generales, pero **no existe un perfil consolidado y de acceso abierto para datos de aprendizaje de lenguas anclados a descriptores del MCER**. Esa ausencia impide comparar evidencias entre productos y convierte cada plataforma en un silo. La tesis propone y publica dicho perfil como resultado secundario, alineable además con ESCO para la portabilidad de la competencia lingüística en el mercado laboral europeo.

### 4.7 Síntesis del vacío de investigación

> **Vacío.** No existe un **método de diseño replicable y validado** que (a) opere sobre descriptores del MCER como unidad de entrada, (b) incorpore la tutoría LLM con una función pedagógica explícitamente delimitada, (c) trate la literacidad en IA como objetivo curricular integrado en la tarea de lengua, y (d) produzca evidencia de desempeño interoperable y anclada al estándar. Esta tesis construye ese método y lo somete a prueba.

---

## 5. Preguntas de investigación, objetivos e hipótesis

### 5.1 Pregunta general

> **PG.** ¿Cómo puede formalizarse un método de diseño replicable —MLLDE— que integre tutores LLM y la literacidad en IA en el diseño curricular anclado al MCER, y qué efectos produce sobre la progresión en descriptores del MCER, la competencia en IA generativa y la autoeficacia de aprendices adultos de lengua?

### 5.2 Preguntas específicas

| # | Pregunta | Se responde en |
|---|---|---|
| **PE1** | ¿Qué componentes, secuencia y reglas de decisión debe contener MLLDE para convertir cualquier descriptor «can-do» del MCER en una lección móvil, de forma que personas diseñadoras distintas produzcan lecciones equivalentes? | Ciclo 1 (Delphi + análisis de replicabilidad) |
| **PE2** | ¿Qué función pedagógica debe tener el tutor LLM dentro del ciclo de la lección, y cómo debe calibrarse su insumo al nivel MCER del aprendiz para preservar la condición *i+1*? | Ciclos 1–2 |
| **PE3** | ¿Produce la integración curricular de la literacidad en IA dentro de la tarea de lengua mejoras significativas en las cuatro competencias de IA generativa, sin coste sobre la progresión lingüística? | Ciclo 2 |
| **PE4** | ¿Qué efecto tiene MLLDE, frente a una condición de uso no estructurado del tutor LLM, sobre la progresión en descriptores del MCER y sobre la autoeficacia del aprendiz? | Ciclo 3 |
| **PE5** | ¿Qué estructura mínima debe tener un perfil xAPI para que la evidencia de desempeño quede anclada a descriptores del MCER y sea comparable entre plataformas? | Transversal, consolidado en Ciclo 3 |

### 5.3 Objetivos

**Objetivo general.** Formalizar, instrumentar y validar empíricamente el método MLLDE como procedimiento replicable de diseño curricular para el aprendizaje móvil de lenguas con tutoría LLM y literacidad en IA integradas, anclado al MCER.

**Objetivos específicos:**

1. **O1 — Formalizar el método.** Especificar los componentes, la secuencia, el contrato de entrada (nivel + descriptor + escenario) y las reglas de decisión de MLLDE en un documento de método verificable, y validarlo mediante panel de personas expertas.
2. **O2 — Delimitar la tutoría LLM.** Definir y probar el contrato pedagógico del tutor LLM: en qué escalón de la escalera de retroalimentación interviene, qué no debe hacer, y cómo se calibra su producción al nivel MCER del aprendiz.
3. **O3 — Integrar la literacidad en IA.** Diseñar y evaluar el módulo de literacidad en IA embebido en la tarea comunicativa, operacionalizando las cuatro competencias del constructo (mecánica de los LLM, *prompting*, verificación de fuentes, autoeficacia) como tareas de recepción, producción y mediación en la lengua meta.
4. **O4 — Especificar la medición.** Construir y publicar el perfil xAPI de datos de aprendizaje de lenguas anclado a descriptores del MCER, con su vocabulario, sus verbos y su mapa a cmi5, y verificar su funcionamiento sobre un LRS real.
5. **O5 — Evaluar el efecto.** Contrastar empíricamente el método frente a una condición de uso no estructurado, en progresión MCER, competencia en IA y autoeficacia, con análisis de equidad entre subgrupos.

### 5.4 Hipótesis

| # | Hipótesis | Contraste |
|---|---|---|
| **H1** | Las lecciones producidas por personas diseñadoras distintas aplicando MLLDE sobre el mismo descriptor MCER presentan una concordancia alta en modo, competencia y tipo de tarea (replicabilidad del método). | Acuerdo interjueces sobre rúbrica de conformidad |
| **H2** | La tutoría LLM delimitada dentro de la escalera de retroalimentación produce mayor progresión en descriptores del MCER que el uso no estructurado del mismo modelo. | Comparación entre condiciones, medida pre/post |
| **H3** | La integración curricular de la literacidad en IA mejora significativamente las cuatro competencias del constructo **sin** deterioro de la progresión lingüística. | Medida pre/post + contraste de no inferioridad |
| **H4** | La retroalimentación no punitiva (ámbar/«revisar», nunca roja; reintento y escalado a tutoría) se asocia a mayor autoeficacia y persistencia en la tarea. | Escala de autoeficacia + métricas de reintento |
| **H5** | Los efectos de H2–H4 no difieren significativamente por edad, género ni experiencia previa con IA (equidad del diseño). | Análisis de moderación por subgrupos |

---

## 6. Metodología

### 6.1 Enfoque general: investigación basada en diseño

La tesis adopta la **investigación basada en diseño (DBR)** porque su objeto es simultáneamente un *artefacto* (el método) y un *conocimiento* (los principios de diseño que lo sostienen). La DBR trabaja en ciclos iterativos de diseño–implementación–análisis–rediseño en contexto real, y produce dos resultados: una intervención que funciona y una teoría local sobre por qué funciona. Internamente, cada ciclo de construcción se ejecuta con **SAM** (Allen & Sites, 2012): fase de preparación, *savvy start* de diseño iterativo y ciclos de construcción.

**Diseño metodológico:** mixto, con integración secuencial explicativa (cuantitativo → cualitativo) en los ciclos 2 y 3.

### 6.2 Los tres macrociclos

| Ciclo | Foco | Objetivos | Métodos | Salida |
|---|---|---|---|---|
| **C1 — Formalización** | El método | O1, O2 | Revisión sistemática de literatura; análisis documental del MCER y del *Plan curricular*; **panel Delphi** (2–3 rondas) con personas expertas en lingüística aplicada, diseño instruccional y tecnología educativa; prueba de replicabilidad con personas diseñadoras independientes | Documento de método MLLDE v1.0 validado + rúbrica de conformidad |
| **C2 — Instrumentación** | El tutor LLM y la literacidad en IA | O2, O3, O4 | Prototipado con SAM; *think-aloud* con aprendices; análisis de la interacción con el tutor; pilotaje del módulo de literacidad en IA; construcción y prueba del perfil xAPI sobre LRS | Prototipo instrumentado + perfil xAPI v0.9 + instrumentos calibrados |
| **C3 — Evaluación** | El efecto | O5 | Estudio cuasi-experimental con dos condiciones (MLLDE vs. uso no estructurado del tutor LLM), medidas pre/post/seguimiento; entrevistas semiestructuradas; análisis de equidad por subgrupos | Evidencia empírica + método MLLDE v2.0 + perfil xAPI v1.0 |

### 6.3 Participantes y contexto

- **Panel de personas expertas (C1):** 12–15 participantes con perfil de investigación en lingüística aplicada, diseño instruccional o tecnología educativa, y experiencia acreditada en alineación al MCER. Selección por criterios, con índice de competencia experta.
- **Personas diseñadoras para la prueba de replicabilidad (C1):** 6–8, sin participación previa en el desarrollo del método; cada una produce una lección a partir del mismo descriptor de entrada.
- **Aprendices (C2–C3):** personas adultas (≥18 años) en niveles **A2–B2**, en dos lenguas meta para verificar el carácter agnóstico del método (español como lengua extranjera e inglés). Muestra orientativa: 20–30 en C2 (pilotaje cualitativo) y **n ≈ 120–160** en C3, repartidos en dos condiciones; el tamaño definitivo se fijará mediante análisis de potencia una vez estimado el tamaño del efecto en C2.
- **Contexto:** entornos de formación de personas adultas y aprendizaje autónomo en dispositivo móvil, con convenios de colaboración a formalizar en el primer año.

> *Todos los tamaños muestrales indicados son orientativos y se ajustarán tras el análisis de potencia del ciclo 2 y la firma de los convenios.*

### 6.4 Instrumentos y variables

| Constructo | Instrumento | Naturaleza |
|---|---|---|
| Progresión lingüística | Prueba pre/post alineada a descriptores MCER (recepción, producción, interacción; mediación en B2), con rúbricas de doble corrección y acuerdo interjueces | Cuantitativa + valorada |
| Conformidad del diseño | Rúbrica de conformidad MLLDE (modo × competencia × nivel × componentes obligatorios) | Cuantitativa |
| Competencia en IA generativa | Instrumento adaptado del constructo de cuatro competencias (mecánica de los LLM, *prompting*, verificación de fuentes, autoeficacia), traducido y validado para el contexto | Cuantitativa |
| Calidad del *prompting* | Rúbrica de valoración de instrucciones producidas por el aprendiz | Valorada |
| Autoeficacia y persistencia | Escala de autoeficacia + métricas conductuales de reintento y abandono extraídas del LRS | Mixta |
| Comportamiento de aprendizaje | Sentencias xAPI ancladas a descriptores del MCER (intentos, escalados a tutoría, tiempo en tarea, ruta de la escalera de retroalimentación) | Cuantitativa |
| Experiencia del aprendiz | *Think-aloud* (C2) y entrevistas semiestructuradas (C3) | Cualitativa |
| Validación del método | Cuestionarios Delphi con consenso por coeficiente de variación e IQR | Mixta |

### 6.5 Análisis de datos

- **Cuantitativo:** estadística descriptiva; contrastes pre/post; **ANCOVA / modelos mixtos** con la puntuación previa como covariable y el centro/grupo como efecto aleatorio; tamaños del efecto con intervalos de confianza; contraste de no inferioridad para H3; análisis de moderación por subgrupos para H5. Corrección por comparaciones múltiples.
- **Cualitativo:** análisis temático reflexivo de *think-alouds* y entrevistas, con codificación doble en una submuestra y reporte de acuerdo.
- **Datos de comportamiento:** análisis de secuencias sobre las sentencias xAPI para reconstruir las rutas reales por la escalera de retroalimentación y su relación con la progresión.
- **Integración:** matriz de convergencia/divergencia entre hallazgos cuantitativos y cualitativos por cada pregunta específica.

### 6.6 Criterios de calidad

Fiabilidad interjueces reportada (κ / CCI) en toda medida valorada; **preinscripción** del plan analítico del ciclo 3 en un repositorio público antes de la recogida de datos; publicación de instrumentos, rúbricas y del perfil xAPI en acceso abierto; auditoría de trazabilidad entre cada afirmación empírica y su dato de origen.

### 6.7 Consideraciones éticas, protección de datos y transparencia de la IA

1. **Comité de ética.** Solicitud de informe favorable al comité de ética de la investigación de la UPV antes del ciclo 2.
2. **Consentimiento informado.** Participación voluntaria, revocable, con información específica sobre el registro de la interacción con el tutor LLM. Exclusión de personas menores de edad.
3. **RGPD.** Minimización de datos, seudonimización en origen, base jurídica de consentimiento, plazos de conservación definidos, sin transferencias no necesarias; evaluación de impacto si procede.
4. **Reglamento Europeo de IA (art. 50).** Divulgación explícita al aprendiz de que interactúa con un sistema de IA y de que determinados contenidos han sido generados o asistidos por IA, con etiquetado dentro de la propia interfaz.
5. **Accesibilidad.** Conformidad WCAG 2.1 AA y Acta Europea de Accesibilidad en todos los materiales de la intervención.
6. **Gobernanza del modelo.** Registro de versiones del modelo y de las instrucciones de sistema, para garantizar la reproducibilidad del estudio pese a la evolución de los proveedores.
7. **Propiedad intelectual.** El MCER, el *Plan curricular del Instituto Cervantes* y las especificaciones xAPI se citan y no se redistribuyen.

### 6.8 Limitaciones previstas

Dependencia de la evolución de los modelos comerciales (mitigada mediante registro de versiones y anclaje del contrato pedagógico a nivel de método, no de proveedor); posible efecto de novedad en la condición experimental (mitigado con medida de seguimiento); dos lenguas meta no agotan la afirmación de agnosticismo lingüístico (se reportará como límite del alcance); autoselección de las personas participantes en contextos de aprendizaje autónomo.

---

## 7. Plan de trabajo y cronograma

Modalidad a **tiempo parcial, cuatro años**, compatible con la actividad profesional de la doctoranda.

| Año | Semestres | Hitos principales | Entregable |
|---|---|---|---|
| **Año 1** | S1–S2 | Revisión sistemática de literatura; análisis documental MCER + *Plan curricular*; formalización de MLLDE v0.9; diseño del Delphi; convenios de colaboración; formación transversal del programa | Documento de método v0.9 · protocolo Delphi · plan de investigación aprobado |
| **Año 2** | S3–S4 | Ejecución del Delphi (2–3 rondas); prueba de replicabilidad; **MLLDE v1.0 validado**; construcción del prototipo instrumentado; perfil xAPI v0.9 sobre LRS; solicitud al comité de ética | **Artículo 1** (el método) enviado · perfil xAPI v0.9 publicado |
| **Año 3** | S5–S6 | Ciclo 2 completo: *think-aloud*, pilotaje del módulo de literacidad en IA, calibración de instrumentos, análisis de potencia; preinscripción del ciclo 3; inicio de la recogida de datos del cuasi-experimento | **Artículo 2** (tutor LLM delimitado + literacidad en IA) enviado · estancia de investigación |
| **Año 4** | S7–S8 | Cierre de la recogida de datos; análisis mixto; entrevistas; MLLDE v2.0; perfil xAPI v1.0; redacción y depósito de la tesis; defensa | **Artículo 3** (evidencia de efecto) enviado · tesis depositada · mención internacional |

**Mención internacional.** Se prevé una estancia de investigación de tres meses en el año 3 en un grupo europeo de referencia en CALL/MALL, y la redacción de al menos una parte de la tesis en inglés, para optar a la mención internacional.

---

## 8. Resultados esperados y contribución original

1. **Un método formalizado y validado (MLLDE v2.0)** — publicado con su documento de especificación, su contrato de entrada, su rúbrica de conformidad y su plantilla de planificación, de modo que un tercer equipo pueda aplicarlo sin la autora.
2. **Un contrato pedagógico para tutores LLM en aprendizaje de lenguas** — la delimitación funcional del modelo dentro de una escalera de retroalimentación, con evidencia empírica de su efecto frente al uso no estructurado.
3. **Un modelo de literacidad en IA integrada en el currículo de lenguas** — operacionalización de las cuatro competencias del constructo como tareas MCER de recepción, producción y mediación, con evidencia de mejora sin coste lingüístico.
4. **Un perfil xAPI abierto para datos de aprendizaje de lenguas anclados al MCER** — vocabulario, verbos y mapa a cmi5, con alineación a ESCO, publicado en acceso abierto.
5. **Evidencia empírica** sobre progresión MCER, competencia en IA y autoeficacia, incluido el análisis de equidad entre subgrupos.
6. **Instrumentos reutilizables** — rúbricas, escalas adaptadas y protocolo de análisis, publicados para su reutilización y réplica.

**Originalidad.** La aportación no está en proponer un marco pedagógico nuevo, sino en **la síntesis operacionalizada, replicable y medible** de marcos consolidados, con dos elementos que la literatura aún no articula conjuntamente: la delimitación funcional del tutor LLM dentro del ciclo didáctico y la integración curricular de la literacidad en IA en la propia tarea de lengua — todo ello anclado a un estándar internacional y verificable mediante datos interoperables.

---

## 9. Plan de difusión

**Revistas objetivo (indexadas):** *ReCALL*; *Computer Assisted Language Learning*; *Language Learning & Technology*; *System*; *Journal of Computer Assisted Learning*; *Computers & Education*; *British Journal of Educational Technology*; *Educación XX1*; *RIED — Revista Iberoamericana de Educación a Distancia*; *Revista Española de Lingüística Aplicada (RESLA)*.

**Congresos:** EUROCALL · WorldCALL · CALL Research Conference · AELFE · AESLA · EDULEARN / INTED · Jornadas de Innovación Educativa y Docencia en Red (UPV).

**Difusión abierta y transferencia:** publicación del método, las rúbricas y el perfil xAPI en repositorio abierto; RiuNet (UPV); ORCID; seminarios de formación docente y transferencia a instituciones de enseñanza de lenguas.

---

## 10. Recursos, viabilidad y encaje institucional

**Viabilidad técnica.** La doctoranda administra un LMS (Chamilo) desde 2019, produce contenido en Moodle y Canvas LMS, empaqueta en SCORM/xAPI desde Articulate 360 (Rise) y ha construido un prototipo funcional del producto de referencia. La infraestructura de recogida de datos (LRS + perfil xAPI) es, por tanto, alcanzable con recursos modestos.

**Viabilidad de acceso al campo.** Más de veinte años de docencia de lenguas a personas adultas y la acreditación como examinadora DELE del Instituto Cervantes facilitan el acceso a poblaciones de aprendices adultos y a instituciones colaboradoras.

**Recursos necesarios:** acceso a un LRS (opción de código abierto autoalojado); créditos de API de un proveedor de LLM para la condición experimental; licencias de software estadístico (alternativas abiertas disponibles); financiación de la estancia de investigación y de las cuotas de publicación en acceso abierto — se concurrirá a las convocatorias de ayudas predoctorales y de movilidad.

**Encaje con la UPV.** La propuesta se inscribe con naturalidad en el Departamento de Lingüística Aplicada de la UPV: continúa la formación de máster de la doctoranda en ese mismo departamento, se apoya en el modelo IPO gamificado desarrollado en él y conecta con la investigación en escritura académica y metadiscurso en la que la doctoranda ya ha participado.

---

## 11. Referencias (APA 7.ª)

Advanced Distributed Learning Initiative. (2017). *xAPI profiles specification* (Version 1.0). GitHub. https://adlnet.github.io/xapi-profiles/

Allen, M. W., & Sites, R. (2012). *Leaving ADDIE for SAM: An agile model for developing the best learning experiences*. ASTD Press.

Casañ-Pitarch, R. (2017). *An approach to digital game-based learning: Video-games principles for language learning*. Journal of Language Teaching and Research.

Clothier, P. (2026). *Mastering mobile learning design: A practical guide* (1st ed.). Routledge.

Council of Europe. (2020). *Common European Framework of Reference for Languages: Learning, teaching, assessment — Companion volume*. Council of Europe Publishing. https://www.coe.int/lang-cefr

Coyle, D. (2007). Content and language integrated learning: Towards a connected research agenda for CLIL pedagogies. *International Journal of Bilingual Education and Bilingualism, 10*(5), 543–562.

Coyle, D., Hood, P., & Marsh, D. (2010). *CLIL: Content and language integrated learning*. Cambridge University Press.

Crawford, M. L. (2001). *Teaching contextually: Research, rationale, and techniques for improving student motivation and achievement in mathematics and science*. CCI Publishing / CORD.

European Commission. (n.d.). *ESCO: European Skills, Competences, Qualifications and Occupations*. Retrieved September 5, 2026, from https://esco.ec.europa.eu/

Europass. (n.d.). *Common European Framework of Reference for language skills* [Self-assessment grid]. European Union. Retrieved September 5, 2026, from https://europass.europa.eu/en/common-european-framework-reference-language-skills

Harmer, J. (2007). *The practice of English language teaching* (4th ed.). Pearson Longman.

IEEE. (2023). *IEEE standard for learning technology — JSON data model format and RESTful web service for learner experience data tracking and access (xAPI)* (IEEE Std 9274.1.1-2023). IEEE Standards Association.

Instituto Cervantes. (n.d.). *Plan curricular del Instituto Cervantes. Niveles de referencia para el español*. Centro Virtual Cervantes. https://cvc.cervantes.es/ensenanza/biblioteca_ele/plan_curricular/default.htm

Johnson, E. B. (2002). *Contextual teaching and learning: What it is and why it's here to stay*. Corwin Press.

Kasper, G., & Rose, K. R. (2001). *Pragmatics in language teaching*. Cambridge University Press.

Kirkpatrick, J. D., & Kirkpatrick, W. K. (2016). *Kirkpatrick's four levels of training evaluation*. ATD Press.

Krashen, S. D. (1985). *The input hypothesis: Issues and implications*. Longman.

Lewis, M. (1993). *The lexical approach: The state of ELT and a way forward*. Language Teaching Publications.

Mayer, R. E. (2009). *Multimedia learning* (2nd ed.). Cambridge University Press.

Phillips, J. J., & Phillips, P. P. (2016). *Handbook of training evaluation and measurement methods* (4th ed.). Routledge.

Ryan, R. M., & Deci, E. L. (2000). Self-determination theory and the facilitation of intrinsic motivation, social development, and well-being. *American Psychologist, 55*(1), 68–78.

Witt, S. M., & Young, S. J. (2000). Phone-level pronunciation scoring and assessment for interactive language learning. *Speech Communication, 30*(2–3), 95–108. https://doi.org/10.1016/S0167-6393(99)00044-8

> **Nota sobre las referencias.** Las entradas de esta lista proceden de la base bibliográfica verificada del proyecto MLLDE. Antes del depósito formal de la propuesta debe **verificarse en la fuente original** la paginación y el año exactos de Casañ-Pitarch (2017), Coyle (2007) y Crawford (2001), y ampliarse el estado de la cuestión (§4.4 y §4.5) con la literatura sobre tutores LLM publicada entre 2024 y 2026, que evoluciona con rapidez.

---

*© 2026 Ana Eslava-Graterol (ProfeAnaEslavaEdTech). Marca y web: profeanaeslava · GitHub: profeanaeslavaedtech · Universitat Politècnica de València. Este documento aplica la metodología MLLDE; «Language Passport»™ y «Grace» son marcas de la autora. Elaborado con asistencia de IA (Claude Code, Anthropic) bajo supervisión, verificación y autoría intelectual humana, conforme a las obligaciones de transparencia del Reglamento Europeo de Inteligencia Artificial.*
