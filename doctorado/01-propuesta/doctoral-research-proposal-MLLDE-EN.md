<!--
  Doctoral research proposal — MLLDE.
  © 2026 Ana Eslava-Graterol (ProfeAnaEslavaEdTech). All Rights Reserved.
  "Language Passport"™ and "Grace" are marks of the author. MLLDE is the underlying methodology.
  CEFR (Council of Europe), Plan curricular (Instituto Cervantes), xAPI (ADL/IEEE),
  ESCO (European Union) and IPA are cited standards, not redistributed.
-->

# DOCTORAL RESEARCH PROPOSAL

## MLLDE — *Mobile Language Learning Design Environment*
### A method for integrating LLM tutors and AI literacy into CEFR curriculum design

---

| | |
|---|---|
| **Candidate** | Ana Zoraida Eslava-Graterol |
| **Contact** | profeanaeslava@gmail.com · https://www.linkedin.com/in/anaeslava |
| **Programme** | PhD Programme — Applied Linguistics |
| **Department** | Department of Applied Linguistics, Universitat Politècnica de València (UPV), Spain |
| **Research line** | Language technologies, instructional design and mobile-assisted language learning |
| **Proposed mode** | Part-time (4 years), compatible with professional activity |
| **Date** | September 2026 |
| **Version** | 1.0 |

> *This proposal develops and empirically validates the MLLDE method, of which the author is the owner. "Language Passport"™ and "Grace" are marks of the author; MLLDE is the underlying methodology. The CEFR (Council of Europe), the Plan curricular del Instituto Cervantes, xAPI (ADL/IEEE), ESCO (European Union) and IPA are cited standards, not redistributed.*

---

## 1. Abstract

Mobile-assisted language learning (MALL) and conversational tutors built on large language models (LLMs) have spread with remarkable speed, yet their incorporation into classrooms and curricula remains **craft-based, non-replicable and hard to evaluate**. Three things are missing at once: (i) a **design procedure** that systematically turns a CEFR can-do descriptor into a playable mobile lesson; (ii) a treatment of **generative-AI literacy** as an *explicit curricular objective* for the language learner rather than a by-product of tool use; and (iii) an **interoperable learning-data architecture** (xAPI/cmi5) that anchors every performance evidence to a CEFR descriptor and makes results comparable across languages, institutions and platforms.

This thesis proposes, formalises and empirically validates **MLLDE (Mobile Language Learning Design Environment)**: a replicable, language-agnostic design method articulating the gamified IPO cycle (Casañ-Pitarch, 2017), the CLIL 4Cs (Coyle, 2007), contextual teaching and learning (Johnson, 2002; Crawford, 2001), the lexical approach (Lewis, 1993) and mobile learning design principles (Clothier, 2026), **anchored throughout to the CEFR modes and competences** (Council of Europe, 2020) and, for Spanish, to the *Plan curricular del Instituto Cervantes*. On that scaffold the method adds two new elements: an **LLM tutor with a bounded pedagogical role** inside a non-punitive feedback ladder, and an **AI-literacy module** embedded in the lesson sequence itself.

The research is designed as **design-based research (DBR)** across three iterative macro-cycles, using mixed methods: expert-panel validation of the method (Delphi), an intervention with adult language learners at A2–B2, and outcome measurement on three planes — CEFR descriptor progression, generative-AI competence, and self-efficacy. Expected outputs are a formalised, validated method, an open xAPI profile specification for CEFR-anchored language-learning data, and empirical evidence on the effect of pedagogically bounded LLM tutoring versus unstructured use.

**Keywords:** CEFR · MALL · LLM tutors · AI literacy · instructional design · design-based research · xAPI · CLIL · gamification · language learning.

---

## 2. Rationale and motivation

Three observations — one professional, two academic — motivate this proposal.

**2.1 The professional observation.** Across more than twenty years designing and delivering language education — 1,568 accredited university teaching hours, LMS administration since 2019, and the end-to-end design of CEFR-aligned gamified courses — the recurring problem has never been a shortage of content or of technology, but the **absence of a procedure**. Every course is redesigned from scratch; every teacher reinvents the sequence; design knowledge does not accumulate. The *Academic Writing Journey* project (rated 10/10 for inclusive design, UPV, 2026) showed that an explicit, documented pedagogical cycle *is* reusable — and that is the seed of MLLDE.

**2.2 The observation about LLM tutors.** Language models have made technically trivial what used to be expensive: unlimited conversational interaction, with immediate correction, in the target language. But *talking to a model* is not *learning a language*. Without an explicit pedagogical contract, an LLM tutor tends to (a) solve the task instead of scaffolding it, (b) produce input that is not calibrated to the learner's level, breaking the *i+1* condition (Krashen, 1985), and (c) displace authentic assessment into an interaction that leaves no recordable evidence. The relevant question is no longer *whether* to use an LLM tutor, but **within which limits, at which step of the learning cycle, and under which evidence record**.

**2.3 The observation about AI literacy.** The Carnegie Mellon study on generative-AI competency identifies four measurable competencies — knowledge of LLM mechanics, prompt engineering, fact and source checking, and self-efficacy — and shows that a short, asynchronous intervention with learn-by-doing practice and immediate explanatory feedback produces significant and demographically equitable gains. That literacy, however, is currently taught in separate courses, disconnected from content. In a language classroom, where the learner is **already using** the model as an interlocutor, there is a singular opportunity: teaching learners to critically evaluate the model's output is **simultaneously** a reception task, a mediation task and an exercise in pragmatic competence in the target language. AI literacy does not compete with the language curriculum — it can be **anchored inside it**.

**2.4 The regulatory frame.** The European AI Act, and specifically its transparency obligations (Art. 50), together with the GDPR and the European Accessibility Act, turn traceability and disclosure of AI-generated content into a design requirement rather than an afterthought. A design method published today must carry that layer from the outset. MLLDE does.

---

## 3. State of the art

### 3.1 The CEFR as a competence core, not a level label

The Common European Framework of Reference (Council of Europe, 2020) replaces the four traditional skills with **four modes of communication** — reception, production, interaction and mediation — sustained by **three communicative competences** — linguistic, sociolinguistic and pragmatic — and describes progress through can-do descriptors across six levels (A1–C2). In industry practice, however, the CEFR is used mostly as a **commercial level label** ("a B1 course") rather than as a **design specification**. Very few products declare, per task, which mode and which competence it develops and against which descriptor the outcome is measured. That weak use of the standard is the direct cause of cross-platform incomparability of results.

### 3.2 MALL: demonstrated efficacy, under-documented design

The mobile language learning literature evidences gains in accessibility, microlearning and distributed practice, and Clothier (2026) systematises mobile design principles: context-driven design, brevity and scanability, learner empathy, with microlearning, storytelling, gamification and performance support as strategies. What the literature documents far less often is **the procedure**: how one moves from a curricular objective to a specific mobile lesson in a way another team could reproduce. Without that link, efficacy evidence is not transferable.

### 3.3 Gamification and content–language integration

Casañ-Pitarch's (2017) IPO model (*Input–Processing–Output*) contributes a gamified learning cycle with a ring architecture and a disciplinary-identity storyline; Coyle's 4Cs (2007, 2010) — content, communication, cognition, culture — contribute integration; ESA (Harmer, 2007) contributes staging (*Engage–Study–Activate*); CTL and the REACT strategies (Johnson, 2002; Crawford, 2001) contribute task authenticity and transfer; the lexical approach (Lewis, 1993) contributes teaching in chunks; the cognitive theory of multimedia learning (Mayer, 2009) contributes dual-coded vocabulary; and interlanguage pragmatics (Kasper & Rose, 2001) contributes the explicit treatment of register and politeness. **All the pieces exist; the operationalised synthesis does not.** MLLDE is that synthesis, and its originality lies in the replicable assembly, not in inventing a new framework.

### 3.4 LLM tutors in language learning

Recent research on LLM-based conversational tutors has focused on correction quality, learner perception and reduced communicative anxiety. Three gaps persist: **input calibration** to the learner's CEFR level, the **functional bounding** of the tutor within the didactic sequence (does it correct? explain? assess? replace the task?), and the **recordability** of the interaction as learning evidence. MLLDE addresses all three through a **feedback ladder** in which the model intervenes only at the last rung, after deterministic rules and the deep-linked reference grammar.

### 3.5 Generative-AI literacy

The Carnegie Mellon study defines a measurable four-competency construct and validates an intervention design — asynchronous modules, learn-by-doing, immediate explanatory feedback — with significant and equitable results. Transferred to language education, that construct is **teachable inside the communicative task itself**, not outside it: verifying the model's output is a critical-reception task; reformulating an instruction is a production task; explaining to another person why the model's answer was inadequate is, in CEFR terms, **mediation** — the very mode the framework places at B2 and above.

### 3.6 Interoperable learning data

xAPI (ADL, 2017; IEEE 9274.1.1-2023) and cmi5 make it possible to record learning experiences outside the LMS and store them in an LRS. Published xAPI profiles cover general domains, but **no consolidated, openly available profile exists for language-learning data anchored to CEFR descriptors**. That absence prevents cross-product comparison of evidence and turns every platform into a silo. This thesis proposes and publishes such a profile as a secondary output, further alignable with ESCO for the portability of language competence in the European labour market.

### 3.7 The research gap in one paragraph

> **Gap.** No **replicable, validated design method** exists that (a) operates on CEFR descriptors as its input unit, (b) incorporates LLM tutoring with an explicitly bounded pedagogical role, (c) treats AI literacy as a curricular objective embedded in the language task, and (d) produces interoperable, standard-anchored performance evidence. This thesis builds that method and puts it to the test.

---

## 4. Research questions, objectives and hypotheses

### 4.1 Overarching question

> **RQ.** How can a replicable design method — MLLDE — be formalised so that it integrates LLM tutors and AI literacy into CEFR-anchored curriculum design, and what effects does it produce on CEFR descriptor progression, generative-AI competence and self-efficacy in adult language learners?

### 4.2 Specific questions

| # | Question | Answered in |
|---|---|---|
| **SQ1** | Which components, sequence and decision rules must MLLDE contain to turn any CEFR can-do descriptor into a mobile lesson, such that different designers produce equivalent lessons? | Cycle 1 (Delphi + replicability test) |
| **SQ2** | What pedagogical role should the LLM tutor hold inside the lesson cycle, and how should its input be calibrated to the learner's CEFR level to preserve the *i+1* condition? | Cycles 1–2 |
| **SQ3** | Does embedding AI literacy inside the language task produce significant gains across the four generative-AI competencies, at no cost to linguistic progression? | Cycle 2 |
| **SQ4** | What effect does MLLDE have, compared with unstructured use of the same LLM tutor, on CEFR descriptor progression and on learner self-efficacy? | Cycle 3 |
| **SQ5** | What minimal structure must an xAPI profile have for performance evidence to be anchored to CEFR descriptors and comparable across platforms? | Cross-cutting, consolidated in Cycle 3 |

### 4.3 Objectives

**General objective.** To formalise, instrument and empirically validate MLLDE as a replicable curriculum-design procedure for mobile language learning with integrated LLM tutoring and AI literacy, anchored to the CEFR.

**Specific objectives:**

1. **O1 — Formalise the method.** Specify MLLDE's components, sequence, input contract (level + descriptor + scenario) and decision rules in a verifiable method document, and validate it through an expert panel.
2. **O2 — Bound the LLM tutor.** Define and test the tutor's pedagogical contract: at which rung of the feedback ladder it intervenes, what it must not do, and how its output is calibrated to the learner's CEFR level.
3. **O3 — Integrate AI literacy.** Design and evaluate the AI-literacy module embedded in the communicative task, operationalising the four construct competencies (LLM mechanics, prompting, source checking, self-efficacy) as reception, production and mediation tasks in the target language.
4. **O4 — Specify the measurement.** Build and publish the xAPI profile for CEFR-anchored language-learning data — vocabulary, verbs and cmi5 mapping — and verify it against a live LRS.
5. **O5 — Evaluate the effect.** Empirically contrast the method against an unstructured-use condition on CEFR progression, AI competence and self-efficacy, including subgroup equity analysis.

### 4.4 Hypotheses

| # | Hypothesis | Test |
|---|---|---|
| **H1** | Lessons produced by different designers applying MLLDE to the same CEFR descriptor show high agreement in mode, competence and task type (method replicability). | Inter-rater agreement on a conformance rubric |
| **H2** | Bounded LLM tutoring inside the feedback ladder yields greater CEFR descriptor progression than unstructured use of the same model. | Between-condition comparison, pre/post |
| **H3** | Curricular integration of AI literacy significantly improves all four construct competencies **without** degrading linguistic progression. | Pre/post measures + non-inferiority test |
| **H4** | Non-punitive feedback (amber / "needs review", never red; retry and escalation to tutoring) is associated with higher self-efficacy and task persistence. | Self-efficacy scale + retry metrics |
| **H5** | The effects in H2–H4 do not differ significantly by age, gender or prior AI experience (design equity). | Subgroup moderation analysis |

---

## 5. Methodology

### 5.1 Overall approach: design-based research

The thesis adopts **design-based research (DBR)** because its object is simultaneously an *artefact* (the method) and a *body of knowledge* (the design principles that sustain it). DBR proceeds through iterative design–implementation–analysis–redesign cycles in a real context, and yields two outputs: an intervention that works and a local theory of why it works. Internally, each build cycle is executed with **SAM** (Allen & Sites, 2012): a preparation phase, an iterative design "savvy start", and build cycles.

**Design:** mixed methods, with explanatory sequential integration (quantitative → qualitative) in cycles 2 and 3.

### 5.2 The three macro-cycles

| Cycle | Focus | Objectives | Methods | Output |
|---|---|---|---|---|
| **C1 — Formalisation** | The method | O1, O2 | Systematic literature review; documentary analysis of the CEFR and the *Plan curricular*; **Delphi panel** (2–3 rounds) with experts in applied linguistics, instructional design and educational technology; replicability test with independent designers | Validated MLLDE method document v1.0 + conformance rubric |
| **C2 — Instrumentation** | LLM tutor and AI literacy | O2, O3, O4 | SAM prototyping; learner think-alouds; tutor-interaction analysis; AI-literacy module pilot; xAPI profile build and LRS testing | Instrumented prototype + xAPI profile v0.9 + calibrated instruments |
| **C3 — Evaluation** | The effect | O5 | Quasi-experimental study with two conditions (MLLDE vs. unstructured LLM tutor use), pre/post/follow-up measures; semi-structured interviews; subgroup equity analysis | Empirical evidence + MLLDE v2.0 + xAPI profile v1.0 |

### 5.3 Participants and setting

- **Expert panel (C1):** 12–15 participants with a research profile in applied linguistics, instructional design or educational technology, and demonstrated experience in CEFR alignment. Criterion sampling with an expert-competence index.
- **Designers for the replicability test (C1):** 6–8, with no prior involvement in developing the method; each produces one lesson from the same input descriptor.
- **Learners (C2–C3):** adults (18+) at **A2–B2**, in two target languages to verify the method's language-agnostic claim (Spanish as a foreign language, and English). Indicative sample: 20–30 in C2 (qualitative pilot) and **n ≈ 120–160** in C3 across two conditions; the final size will be set by a power analysis once the effect size is estimated in C2.
- **Setting:** adult education and self-directed mobile learning environments, with collaboration agreements to be formalised in year 1.

> *All sample sizes stated are indicative and will be adjusted after the cycle-2 power analysis and the signing of collaboration agreements.*

### 5.4 Instruments and variables

| Construct | Instrument | Nature |
|---|---|---|
| Linguistic progression | CEFR-descriptor-aligned pre/post assessment (reception, production, interaction; mediation at B2), double-marked with inter-rater agreement | Quantitative + rated |
| Design conformance | MLLDE conformance rubric (mode × competence × level × mandatory components) | Quantitative |
| Generative-AI competence | Instrument adapted from the four-competency construct (LLM mechanics, prompting, source checking, self-efficacy), translated and validated for the setting | Quantitative |
| Prompting quality | Rubric scoring of learner-produced prompts | Rated |
| Self-efficacy and persistence | Self-efficacy scale + behavioural retry/abandonment metrics from the LRS | Mixed |
| Learning behaviour | CEFR-descriptor-anchored xAPI statements (attempts, escalations to tutoring, time on task, path through the feedback ladder) | Quantitative |
| Learner experience | Think-alouds (C2) and semi-structured interviews (C3) | Qualitative |
| Method validation | Delphi questionnaires with consensus by coefficient of variation and IQR | Mixed |

### 5.5 Data analysis

- **Quantitative:** descriptive statistics; pre/post contrasts; **ANCOVA / mixed models** with baseline score as covariate and site/group as a random effect; effect sizes with confidence intervals; non-inferiority testing for H3; subgroup moderation analysis for H5. Correction for multiple comparisons.
- **Qualitative:** reflexive thematic analysis of think-alouds and interviews, with double coding on a subsample and reported agreement.
- **Behavioural data:** sequence analysis over xAPI statements to reconstruct actual paths through the feedback ladder and their relation to progression.
- **Integration:** a convergence/divergence matrix between quantitative and qualitative findings for each specific question.

### 5.6 Quality criteria

Reported inter-rater reliability (κ / ICC) for every rated measure; **pre-registration** of the cycle-3 analysis plan in a public repository before data collection; open publication of instruments, rubrics and the xAPI profile; an audit trail linking every empirical claim to its source data.

### 5.7 Ethics, data protection and AI transparency

1. **Ethics committee.** A favourable report will be sought from the UPV research ethics committee before cycle 2.
2. **Informed consent.** Voluntary, revocable participation, with specific information about the recording of LLM tutor interactions. Minors excluded.
3. **GDPR.** Data minimisation, pseudonymisation at source, consent as legal basis, defined retention periods, no unnecessary transfers; impact assessment if applicable.
4. **European AI Act (Art. 50).** Explicit disclosure to the learner that they are interacting with an AI system and that specified content is AI-generated or AI-assisted, labelled inside the interface itself.
5. **Accessibility.** WCAG 2.1 AA and European Accessibility Act conformance across all intervention materials.
6. **Model governance.** Versioning of the model and of system instructions, so the study remains reproducible despite provider evolution.
7. **Intellectual property.** The CEFR, the *Plan curricular del Instituto Cervantes* and the xAPI specifications are cited, not redistributed.

### 5.8 Anticipated limitations

Dependence on the evolution of commercial models (mitigated by version logging and by anchoring the pedagogical contract at method rather than provider level); a possible novelty effect in the experimental condition (mitigated by a follow-up measure); two target languages do not exhaust the language-agnostic claim (reported as a scope limitation); self-selection of participants in self-directed learning settings.

---

## 6. Work plan and timeline

**Part-time mode, four years**, compatible with the candidate's professional activity.

| Year | Semesters | Main milestones | Deliverable |
|---|---|---|---|
| **Year 1** | S1–S2 | Systematic literature review; documentary analysis of CEFR + *Plan curricular*; MLLDE v0.9 formalisation; Delphi design; collaboration agreements; programme's transferable-skills training | Method document v0.9 · Delphi protocol · approved research plan |
| **Year 2** | S3–S4 | Delphi execution (2–3 rounds); replicability test; **validated MLLDE v1.0**; instrumented prototype build; xAPI profile v0.9 on an LRS; ethics committee submission | **Paper 1** (the method) submitted · xAPI profile v0.9 published |
| **Year 3** | S5–S6 | Full cycle 2: think-alouds, AI-literacy module pilot, instrument calibration, power analysis; cycle-3 pre-registration; start of quasi-experimental data collection | **Paper 2** (bounded LLM tutor + AI literacy) submitted · research stay |
| **Year 4** | S7–S8 | Close data collection; mixed analysis; interviews; MLLDE v2.0; xAPI profile v1.0; thesis writing and deposit; viva | **Paper 3** (effect evidence) submitted · thesis deposited · international mention |

**International mention.** A three-month research stay in year 3 at a European reference group in CALL/MALL is foreseen, together with writing at least part of the thesis in English, to qualify for the international mention.

---

## 7. Expected outcomes and original contribution

1. **A formalised, validated method (MLLDE v2.0)** — published with its specification document, input contract, conformance rubric and planning template, such that a third-party team can apply it without the author.
2. **A pedagogical contract for LLM tutors in language learning** — the functional bounding of the model inside a feedback ladder, with empirical evidence of its effect against unstructured use.
3. **A model of AI literacy integrated into the language curriculum** — the four construct competencies operationalised as CEFR reception, production and mediation tasks, with evidence of gains at no linguistic cost.
4. **An open xAPI profile for CEFR-anchored language-learning data** — vocabulary, verbs and cmi5 mapping, ESCO-aligned, published openly.
5. **Empirical evidence** on CEFR progression, AI competence and self-efficacy, including subgroup equity analysis.
6. **Reusable instruments** — rubrics, adapted scales and the analysis protocol, published for reuse and replication.

**Originality.** The contribution is not a new pedagogical framework but **the operationalised, replicable and measurable synthesis** of established ones, with two elements the literature has not yet articulated together: the functional bounding of the LLM tutor inside the didactic cycle, and the curricular integration of AI literacy into the language task itself — all anchored to an international standard and verifiable through interoperable data.

---

## 8. Dissemination plan

**Target (indexed) journals:** *ReCALL*; *Computer Assisted Language Learning*; *Language Learning & Technology*; *System*; *Journal of Computer Assisted Learning*; *Computers & Education*; *British Journal of Educational Technology*; *Educación XX1*; *RIED — Revista Iberoamericana de Educación a Distancia*; *Revista Española de Lingüística Aplicada (RESLA)*.

**Conferences:** EUROCALL · WorldCALL · CALL Research Conference · AELFE · AESLA · EDULEARN / INTED · UPV Educational Innovation and Networked Teaching conference.

**Open dissemination and transfer:** open-repository release of the method, rubrics and xAPI profile; RiuNet (UPV); ORCID; teacher-training seminars and transfer to language-teaching institutions.

---

## 9. Resources, feasibility and institutional fit

**Technical feasibility.** The candidate has administered an LMS (Chamilo) since 2019, produces content on Moodle and Canvas LMS, packages SCORM/xAPI from Articulate 360 (Rise), and has built a working prototype of the reference product. The data-collection infrastructure (LRS + xAPI profile) is therefore achievable on modest resources.

**Field-access feasibility.** More than twenty years teaching languages to adults and accreditation as an Instituto Cervantes DELE examiner facilitate access to adult learner populations and to collaborating institutions.

**Resources required:** access to an LRS (self-hosted open-source option); LLM provider API credits for the experimental condition; statistical software licences (open alternatives available); funding for the research stay and open-access publication fees — pre-doctoral and mobility funding calls will be applied for.

**Fit with UPV.** The proposal sits naturally within UPV's Department of Applied Linguistics: it continues the candidate's master's training in that same department, builds on the gamified IPO model developed there, and connects with the academic-writing and metadiscourse research in which the candidate has already taken part.

---

## 10. References (APA 7th)

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

> **Note on the references.** The entries above come from the MLLDE project's verified bibliographic base. Before formal deposit of the proposal, the exact pagination and year of Casañ-Pitarch (2017), Coyle (2007) and Crawford (2001) should be **verified against the original sources**, and the state of the art (§3.4 and §3.5) expanded with the fast-moving 2024–2026 literature on LLM tutors.

---

*© 2026 Ana Eslava-Graterol (ProfeAnaEslavaEdTech). Brand & website: profeanaeslava · GitHub: profeanaeslavaedtech · Universitat Politècnica de València. This document applies the MLLDE methodology; "Language Passport"™ and "Grace" are marks of the author. Prepared with AI assistance (Claude Code, Anthropic) under human supervision, verification and intellectual authorship, in line with the transparency obligations of the European AI Act.*
