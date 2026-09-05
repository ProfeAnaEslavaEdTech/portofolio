<!--
  Doctoral research proposal — MLLDE, the voice tutor and three tiers of evidence.
  Integrates the author's own document "MLLDE y el tutor por voz: los tres tiers de evidencia"
  (2026-09-05) as the technical core, inside the full apparatus of a doctoral proposal.
  © 2026 Ana Eslava-Graterol (MLLDE, UPV). TK Coach and "Capi" © Talketika.
  CEFR (Council of Europe), xAPI (ADL/IEEE), IPA, ESCO: cited standards, not redistributed.
-->

# DOCTORAL RESEARCH PROPOSAL

## MLLDE — *Multimodal Language Learning Design & Evaluation*
### Modality-declared curriculum design for mobile language learning, and speaking assessment with three tiers of evidence

---

| | |
|---|---|
| **Candidate** | Ana Zoraimy Eslava Graterol |
| **Contact** | profeanaeslava@gmail.com · linkedin.com/in/anaeslava |
| **Programme** | PhD Programme — Applied Linguistics |
| **Department** | Department of Applied Linguistics, Universitat Politècnica de València (UPV), Spain |
| **Research line** | Language technologies, speaking assessment and CEFR-anchored instructional design |
| **Application case** | TK Coach / "Capi" — business-English voice tutor (Talketika) |
| **Proposed mode** | Part-time (4 years), compatible with professional activity |
| **Date · version** | September 2026 · v2.0 |

> **MLLDE** — *Multimodal Language Learning Design & Evaluation*. The author's method and evaluation framework, whose **Measurement Module** this proposal develops and validates. "TK Coach" and "Capi" are marks of Talketika; the CEFR (Council of Europe), xAPI (ADL/IEEE), IPA and ESCO are cited standards, not redistributed.

---

## 1. Abstract

A generative model is **fluent by design**: it will produce a plausible score whether or not it is entitled to, and that fluency is precisely what disqualifies it as an assessor. The problem this thesis addresses is therefore methodological before it is technical: **how to turn a learner's real spoken production in front of an AI agent into evidence of competence traceable to the CEFR, without the model inventing the grade.**

The proposed and validated answer is **MLLDE** (*Multimodal Language Learning Design & Evaluation*), a method with **two inseparable pillars**:

- **The Design pillar.** A replicable procedure for building mobile language curriculum in which **modality** — text, audio, image, **voice** — is not packaging but a **declared design variable**: every step of a lesson states which modality carries the input, the practice and the production, and against which CEFR mode and descriptor it is measured.
- **The Evaluation pillar.** The **Measurement Module**, which turns what the learner produces — above all spoken production in front of an agent — into CEFR-traceable evidence.

Both share one architecture, and the evaluation pillar rests on three decisions:

1. **Measure ≠ Decide.** The model **observes and describes** what happens in the interaction; a **deterministic engine** — code, not AI — **computes** the band from those observations. Nothing on screen is invented by a model.
2. **Engine + pack.** The measurement rules are client-agnostic; each product fills a **pack** with its tasks, levels and sound inventory. Applying the module to a second application means **filling a pack, not redesigning** — the replicability claim the thesis must demonstrate.
3. **Three tiers of evidence.** Voice signal is not measurable at uniform precision. Every claim **declares its tier**, so a report never asserts more accuracy than the engine actually has. Pronunciation — the hardest signal — is the test case, and carrying it from Tier 1 to Tier 3 is the thesis's deep phonemic contribution.

Methodologically this is **design-based research with validation in production**: Tier 1 is already deployed and emitting evidence to a Learning Record Store, so the agreement between the LLM-applied rubric and **expert human assessment** can be tested on real rather than simulated data.

**Keywords:** CEFR · speaking assessment · voice tutors · GOP and pronunciation · xAPI · evidence honesty · design-based research · applied linguistics.

---

## 2. Rationale

**2.1 The underlying problem: fluency is not validity.** Conversational tutors have made unlimited speaking practice technically trivial. But a language model placed in the assessor's chair does not distinguish between *describing* a performance and *scoring* it: it produces a band as fluently as it produces a sentence. The result is systems that display figures without traceability, that cannot withstand an audit, and that cannot be compared with one another. MLLDE's answer is not a better prompt but an **architectural separation of responsibilities**.

**2.2 Why pronunciation is the decisive case.** Of all the signals speech emits, pronunciation is the most over-promised in the market and the least methodologically defensible. Measuring it properly requires acoustic instrumentation, and asserting it without that instrumentation is exactly the kind of over-claim this thesis sets out to make impossible. The tier model is therefore not a detour: it is how one states precisely **what can be measured today, what can be measured with instrumentation, and what is still research**.

**2.3 Why three tiers rather than all-or-nothing.** A commercial tutor cannot wait for research to conclude before delivering value; and research cannot be held captive by a demo. Tiers make it possible to **ship with Tier 1** — real voice, honest measurement — while Tier 2 is developed and validated and Tier 3 is researched, each with its own validity design. It is a maturity model for evidence, not an excuse.

**2.4 The professional observation.** More than twenty years designing and delivering language education — 1,568 accredited university teaching hours, LMS administration since 2019, CEFR-aligned gamified courses — show that the bottleneck is neither content nor technology but the **absence of a cumulative procedure**. MLLDE grew from that, and TK Coach is its first complete instantiation.

---

## 3. State of the art

### 3.1 The CEFR as a measurement specification, not a label

The *Companion Volume* (Council of Europe, 2020) organises competence into **modes of communication** — reception, production, interaction and **mediation** — with can-do descriptors per scale and level. In industry practice, however, the CEFR is used as a **commercial label** ("B1 level") and rarely as a **measurement specification**: almost no product declares, per metric, which named scale it measures against. MLLDE imposes the opposite rule: **no metric without a descriptor**, each citing its scale and identifier (IRI) in a single registry.

### 3.2 Automated speech assessment

Machine-assisted assessment of spoken production has two traditions that rarely meet. On one side, **acoustic pronunciation scoring**, whose reference point remains *Goodness of Pronunciation* (Witt & Young, 2000) and its commercial descendants. On the other, **holistic rubric rating**, now within reach of an LLM working over a transcript. The first is precise and narrow; the second is broad and unverifiable. **Neither alone sustains an auditable CEFR-level claim.** This thesis's contribution is to articulate them along an explicit maturity scale — the three tiers — rather than picking one and hiding its limits.

### 3.3 Feedback, noticing and i+1

The input hypothesis (Krashen, 1985) and the noticing hypothesis (Schmidt, 1990) ground the case for feedback that is **dosed by level** rather than uniform. MLLDE operationalises this as a **noticing scale (0–4)** graduating salience within the recast: **model** at A2–B1, **elicit** at B2+. What matters methodologically is who decides what: **code decides the feedback level (0–3); the LLM detects and drafts.**

### 3.4 Intelligibility rather than native accent

The intelligibility literature and the IPA's own position (1999) hold that the defensible target is **intelligible, appropriate speech**, not approximation to a native accent. MLLDE turns this into an engine rule: **accepted variants** (for instance *seseo* / *distinción*) **never** lower a score. It is an ethical decision as much as a technical one, with direct consequences for the Tier 3 phonemic inventory.

### 3.5 Interoperable learning data

xAPI (IEEE Std 9274.1.1-2023) and Learning Record Stores allow experiences to be recorded outside the LMS. What does not exist is a **consolidated, open profile for language-competence evidence anchored to CEFR descriptors**, with explicit declaration of the measurement model and the tier of every claim. Without that, two platforms are not comparable even when both say "B1".

### 3.6 The gap

> No **replicable, auditable method** exists that (a) explicitly separates **observation from decision** in AI-assisted assessment of spoken production, (b) anchors every metric to a named CEFR scale, (c) **declares the precision** of each claim through a tier model, and (d) emits that evidence in an interoperable format allowing sessions, models and products to be compared. This thesis builds it and tests it on a system already in production.

---

## 4. The method: MLLDE and its Measurement Module

### 4.1 Principles

| Principle | What it means operationally |
|---|---|
| **Measure ≠ Decide** | The LLM describes; a deterministic engine computes the band. No figure comes from a generation. |
| **No metric without a descriptor** | Each metric cites a named *Companion Volume* scale and its IRI in a single registry. |
| **Engine + pack** | Client-agnostic rules; each product supplies its tasks, levels and sound inventory. |
| **Five skills** | Reception, production, interaction and **mediation**, all anchored to the *Companion Volume*. |
| **Traceability** | All evidence is recorded as **xAPI** in an LRS, with a pseudonymous actor. |
| **Evidence honesty** | Every claim declares its **tier** and its per-session **measurement model**. |

**Scale.** 0–10 (pass ≥ 6, floors ≥ 4), with a Cambridge 0–5 view by rounding and halving.

### 4.2 The Design pillar: modality as a declared variable

The principle governing measurement governs design too: **nothing implicit**. If measurement requires every metric to cite its descriptor, design requires **every lesson step to declare its modality and its CEFR mode**.

**A lesson's input contract.** CEFR level + can-do descriptor + real-world scenario + **modality profile**. That fourth element is the Design pillar's contribution: the profile states, step by step, which channel carries the input, which supports practice, and in which one production is required.

| Lesson step | CEFR mode | Input modality | Production modality |
|---|---|---|---|
| Arrival — hook and objective | — | text + image | — |
| Vocabulary and chunks | Reception | audio + image (dual coding) | recognition |
| Model dialogue | Reception | **voice** | — |
| Guided practice | Processing | text or audio | text |
| Mission — authentic task | **Interaction** | **voice** (agent) | **voice** |
| Transfer | Production | free | **voice or writing, learner's choice** |
| Culture and pragmatics | — | text + image | — |

**Why this matters for a thesis and not only for a product.** The mobile-learning literature describes *principles* — brevity, context, microlearning — but rarely a **procedure** another team could reproduce, and almost never treats modality as something decided and justified. Declaring it has three testable consequences: the lesson becomes **auditable** (one can check that CEFR mode and channel agree), **replicable** (two designers starting from the same descriptor and profile should produce equivalent lessons) and **measurable** (the evidence each step emits already knows which mode it belongs to).

**Engine + pack, in design too.** The lesson cycle is a shared **engine**; a given lesson is a **data object**. Building a new lesson — or a new language — is **filling in data, not rewriting logic**. It is the same replicability claim that underpins the evaluation pillar, and it faces the same test (RQ6).

**Frameworks the Design pillar synthesises**, all established and none invented: the gamified **IPO** cycle (Casañ-Pitarch, 2017); the **CLIL 4Cs** (Coyle, 2007); **ESA** (Harmer, 2007); **CTL / REACT** (Johnson, 2002; Crawford, 2001) for task authenticity; the **lexical approach** (Lewis, 1993) for teaching in chunks; and the **cognitive theory of multimedia learning** (Mayer, 2009), which is precisely what grounds treating modality as a decision rather than decoration. The originality lies in none of them, but in **the operationalised synthesis and the explicit modality declaration**.

### 4.3 Voice-tutor architecture

The learner practises by **speaking** real workplace situations with "Capi". The measurement loop:

> **Capi (role-play)** → **MLLDE evaluator** (band 0–10 + weak *i+1* descriptor) → **Practice** (drills, cards, mediation) → **Capi** → the band rises **in the next conversation**.

- **Three observing agents** (Capi · corrector · evaluator) and a **consolidator written in code** — not a fourth LLM — which computes the cumulative level (`Global×5 + analytics×2 ÷ pool × 10`) and emits **a single entry** to the LRS. A **writer** drafts the summary; it does not measure. **Generators** create content: code picks the descriptor, the LLM writes it.
- **Two flows that never cross:** *measurement* (once per session: `completed` + rubric) and *pedagogy* (per turn: `adapted` + `pedagogical-action` + `learning-target`). **Correction is pedagogy and never scores** — the firewall that makes the system auditable.
- **Acoustic gate (ASR 0.70).** Below that recognition confidence the turn is logged as an **incident** and does not score. It is the explicit boundary between what is measurable and what is not.

### 4.4 The three tiers of evidence

| Tier | Name | What it measures | How | Status |
|---|---|---|---|---|
| **1** | **Voice rubric** *(measurable today)* | `grammar_accuracy` · `vocabulary_range` · `discourse_management` · `interaction` · `global_achievement` | Rubric-judge over the **ASR transcript**. **Does not measure pronunciation.** | **In production**, verified against a live LRS |
| **2** | **Instrumented** | **Pronunciation** at word and utterance level: intelligibility and appropriacy | Vendor pronunciation assessment (GOP-style acoustic scoring) | **Planned** — acoustic layer |
| **3** | **Custom GOP** *(research)* | **Phonemic pronunciation**: target features per level, accepted variants | **IPA inventory** per level + bespoke acoustic engineering (Witt & Young, 2000) | **Research** — the thesis's deep contribution |

**Cross-cutting rules.** *(i)* A report **declares the tier** of each claim and never asserts the precision of a higher tier; where a skill has no anchored metric it shows **"—"**, never a value (today: pronunciation = "—" until Tier 2). *(ii)* **Intelligibility, not native accent**: accepted variants never lower a score. *(iii)* **Incremental gain**: each tier adds signal without breaking the previous ones. *(iv)* **Comparability**: each session declares its `measure_model`, so sessions from different tiers or models are never mixed.

---

## 5. Research questions, objectives and hypotheses

### 5.1 Questions

| # | Question | Cycle |
|---|---|---|
| **RQ1 · Validity** | Does a CEFR rubric applied by an LLM over an ASR transcript (Tier 1) produce **reliable and stable** bands against expert human assessment? Does it vary with model size? | C1 |
| **RQ2 · Honesty as method** | Does **unifying all surfaces on a single source of truth** (the LRS) work as an anti-hallucination test — if every screen agrees, does the margin hold? | C1–C2 |
| **RQ3 · Feedback** | Does the **noticing scale** — dosing salience by level — improve ***uptake*** (self-repair at B2+, form registration at A2–B1) without raising the affective filter? | C2 |
| **RQ4 · Pronunciation by tier** | What does validity gain in moving Tier 1 → 2 → 3? What is the defensible **intelligibility floor** at each tier? | C2–C3 |
| **RQ5 · Modality-declared design** | Does the **declared modality profile** yield equivalent lessons across different designers starting from the same descriptor? And does the modality choice affect progression in the CEFR mode the lesson sets out to develop? | C1–C2 |
| **RQ6 · Replicability** | Can an independent team instantiate **both the design and the measurement engines** in a second application by **filling a pack**, without touching the engine, and obtain comparable lessons and measures? | C3 |

### 5.2 Objectives

1. **O1** — Formalise the MLLDE Measurement Module (principles, scale registry, pack schema, consolidator rules) into a specification third parties can verify.
2. **O2** — Establish **Tier 1 validity**: agreement with expert human assessment, test-retest stability, and sensitivity to model size.
3. **O3** — Instrument and validate **Tier 2**, switching on the pronunciation band currently shown as "—", and determine its intelligibility floor.
4. **O4** — Develop **Tier 3**: an IPA inventory per level with accepted variants, and a bespoke GOP that is explainable and does not penalise legitimate varieties.
5. **O5** — Formalise the **Design pillar**: input contract with modality profile, planning template and conformance rubric, validated through an expert panel and a designer-equivalence test.
6. **O6** — Publish the **xAPI profile** for CEFR-anchored competence evidence, carrying tier and measurement-model declarations, and demonstrate **engine + pack** replicability — design and measurement — in a second application.

### 5.3 Hypotheses

| # | Hypothesis | Test |
|---|---|---|
| **H1** | Agreement between the Tier 1 band and expert human assessment reaches reliability acceptable for formative use, and is **stable** on test-retest. | ICC / weighted κ; test-retest |
| **H2** | The Tier 1 band is **sensitive to model size**, which is why `measure_model` must be declared for sessions to be comparable. | Between-model comparison on the same sessions |
| **H3** | Level-dosed noticing increases ***uptake*** relative to uniform feedback, without increasing drop-off. | Between-condition contrast + persistence metrics |
| **H4** | Moving to Tier 2 improves the validity of the pronunciation claim against human intelligibility judgement; Tier 3 additionally makes it **explainable** at phoneme level. | Concurrent validity by tier |
| **H5** | Different designers starting from the same descriptor and modality profile produce lessons with **high agreement** on mode, competence and channel. | Inter-rater agreement on a conformance rubric |
| **H6** | An independent team reproduces comparable **lessons and measures** by **filling a pack**, without modifying the engine. | End-to-end replicability test |

---

## 6. Methodology

### 6.1 Design

**Design-based research with validation in production.** The object is at once an artefact (the module) and a body of knowledge (the principles sustaining it). That Tier 1 is **already deployed** distinguishes this proposal from a laboratory study: the validity data come from real use, not simulation.

| Cycle | Focus | Objectives | Methods |
|---|---|---|---|
| **C1 — Formalisation and Tier 1 validity** | The method, and the measure that already exists | O1, O2, O5 | Formalisation of both pillars; **Delphi panel** on the design contract; **equivalence test** with independent designers; sampling of LRS sessions; **double expert human assessment** with inter-rater agreement; test-retest; model-size sensitivity; integrity audit |
| **C2 — Instrumentation and feedback** | Tier 2 pronunciation + noticing | O3 | Acoustic-layer integration; concurrent validity against intelligibility judgement; uptake study with contrasted salience conditions; think-alouds |
| **C3 — Tier 3 and replicability** | The phonemic contribution, and the test of the method | O4, O6 | IPA inventory per level; bespoke GOP; phonemic validation; **end-to-end replicability test** (design + measurement) with an independent team filling a pack; publication of the xAPI profile |

### 6.2 Data and instruments

- **Learning evidence:** **xAPI** statements in an **LRS** (Veracity), **pseudonymous actor**, two separated flows (measurement / pedagogy), ASR gate 0.70, and the extensions `ext/effective-time`, `ext/measure-model`, `ext/srs-schedule`, `ext/learning-target`.
- **Human criterion:** a panel of expert raters with CEFR training, blind double marking on a subsample, and reported agreement.
- **Pronunciation:** human intelligibility judgements as the external criterion for Tiers 2 and 3.
- **Integrity audit:** a measurement audit with a findings matrix, an ***"H0 watchdog"*** verifying that **no descriptor is ever painted as a band**, and verification in production.
- **Transfer instruments:** per-person reports (learner / teacher / HR) under the Kirkpatrick and Phillips frameworks, with optional **ESCO** alignment.

### 6.3 Analysis

Inter-rater reliability (ICC, weighted κ) and LLM–human agreement; test-retest stability; mixed models for the effect of salience condition on uptake, with site as a random effect; concurrent validity per tier with confidence intervals; sequence analysis over xAPI to reconstruct real trajectories; thematic analysis of think-alouds. **Pre-registration** of each cycle's analysis plan before data collection.

### 6.4 Ethics and compliance

1. **GDPR** (Reg. EU 2016/679): personal data kept out of the model and the LRS; pseudonymisation at source; measurement on a paid service **with no training** on the data.
2. **EU AI Act, Art. 50** (Reg. EU 2024/1689): the agent is declared as AI to the learner; AI-assisted or AI-generated content is labelled.
3. **Intelligibility, not native accent:** an explicit ethical decision — legitimate varieties of English are not penalised.
4. **UPV ethics committee** before cycle 2. Voluntary, revocable participation; minors excluded.
5. **Accessibility:** WCAG 2.1 AA across all intervention surfaces.
6. **Intellectual property:** the CEFR is paraphrased and cited, not reproduced; Cambridge, xAPI (ADL/IEEE), IPA and ESCO are cited as standards.

### 6.5 Anticipated limitations

Dependence on commercial ASR and pronunciation-assessment vendors (mitigated by declaring `measure_model` per session and anchoring the contract to the method rather than the provider); the test case is **business English**, so generalisation to other languages and domains rests on the pack test and must be reported as a scope limitation; self-selection among users of a live product; a possible novelty effect, mitigated by follow-up measures.

---

## 7. Work plan

**Part-time, four years.**

| Year | Milestones | Deliverable |
|---|---|---|
| **1** | Systematic review; formal specification of the Measurement Module and the scale registry; design of the Tier 1 validity study; ethics submission; collaboration agreements | Specification v1.0 · approved research plan |
| **2** | Full cycle 1: LRS sampling, double expert human assessment, test-retest, model-size sensitivity, integrity audit | **Paper 1** — Tier 1 validity · xAPI profile v0.9 |
| **3** | Cycle 2: acoustic-layer integration (Tier 2), concurrent validity, noticing uptake study; research stay | **Paper 2** — instrumented pronunciation and noticing |
| **4** | Cycle 3: IPA inventory and bespoke GOP (Tier 3); engine + pack replicability test; writing, deposit and viva | **Paper 3** — phonemic GOP · thesis deposited · international mention |

**International mention:** a three-month stay in year 3 at a European reference group in speech assessment or CALL, and part of the thesis written in English.

---

## 8. Expected outcomes and original contribution

1. **An open specification of MLLDE in both pillars** — the design contract with its modality profile and conformance rubric, and the Measurement Module with its CEFR scale registry, pack schema and consolidator rules, applicable by third parties.
2. **Tier 1 validity evidence** — agreement with expert human assessment, stability and model sensitivity, on production data.
3. **Pronunciation switched on and explained** — from the honest "—" to instrumented Tier 2 and phonemic Tier 3, with an IPA inventory per level and accepted variants.
4. **An open xAPI profile** for CEFR-anchored competence evidence, carrying tier and measurement-model declarations.
5. **The engine + pack replicability test** in a second application.
6. **An evidence-honesty policy** transferable to any AI-based educational product.

**Originality.** Not a new rubric, nor a new acoustic algorithm, but **an architecture of responsibility**: separating observation from decision, requiring every claim to declare its precision, and making both verifiable in interoperable data. It is a methodological contribution to AI-assisted assessment, with pronunciation as the test case carried through to phoneme level.

---

## 9. Dissemination

**Target journals:** *Language Testing* · *Assessing Speaking / Assessing Writing* · *ReCALL* · *Computer Assisted Language Learning* · *Language Learning & Technology* · *Speech Communication* · *System* · *Computers & Education* · *RESLA* · *Educación XX1*.

**Conferences:** EUROCALL · WorldCALL · Interspeech / SLaTE · ALTE · EALTA · AESLA · AELFE · UPV Educational Innovation conference.

**Open access:** specification, registry, rubrics and xAPI profile in a public repository; RiuNet (UPV); ORCID.

---

## 10. Feasibility and institutional fit

**Technical.** Tier 1 is **in production and verified** against a live LRS; the candidate has administered LMSs since 2019, packages SCORM/xAPI, and built the whole system. The data-collection infrastructure does not need creating — it needs validating.

**Field access.** A real population of adult learners through TK Coach, plus twenty years of teaching and accreditation as an Instituto Cervantes DELE examiner.

**Resources.** LRS (Veracity, already running); LLM and vendor pronunciation-assessment API credits for Tier 2; expert human rater time (the main cost line); open statistical tooling; funding for the research stay and open-access fees — pre-doctoral and mobility calls will be applied for.

**Fit with UPV.** The proposal belongs in the **Department of Applied Linguistics**, where the candidate took her master's and carried out her corpus research on metadiscourse, and where the gamified IPO model informing MLLDE's instructional design was developed.

---

## 11. References (APA 7th)

Advanced Distributed Learning Initiative. (2017). *xAPI profiles specification* (Version 1.0). https://adlnet.github.io/xapi-profiles/

Casañ-Pitarch, R. (2017). *An approach to digital game-based learning: Video-games principles for language learning*. Journal of Language Teaching and Research.

Council of Europe. (2020). *Common European Framework of Reference for Languages: Learning, teaching, assessment — Companion volume*. Council of Europe Publishing.

Coyle, D. (2007). Content and language integrated learning: Towards a connected research agenda for CLIL pedagogies. *International Journal of Bilingual Education and Bilingualism, 10*(5), 543–562.

Crawford, M. L. (2001). *Teaching contextually: Research, rationale, and techniques for improving student motivation and achievement in mathematics and science*. CCI Publishing / CORD.

European Commission. (n.d.). *ESCO: European Skills, Competences, Qualifications and Occupations*. Retrieved September 5, 2026, from https://esco.ec.europa.eu/

IEEE. (2023). *IEEE standard for learning technology — JSON data model format and RESTful web service for learner experience data tracking and access (xAPI)* (IEEE Std 9274.1.1-2023). IEEE Standards Association.

International Phonetic Association. (1999). *Handbook of the International Phonetic Association: A guide to the use of the International Phonetic Alphabet*. Cambridge University Press.

Harmer, J. (2007). *The practice of English language teaching* (4th ed.). Pearson Longman.

Johnson, E. B. (2002). *Contextual teaching and learning: What it is and why it's here to stay*. Corwin Press.

Kirkpatrick, J. D., & Kirkpatrick, W. K. (2016). *Kirkpatrick's four levels of training evaluation*. ATD Press.

Krashen, S. D. (1985). *The input hypothesis: Issues and implications*. Longman.

Lewis, M. (1993). *The lexical approach: The state of ELT and a way forward*. Language Teaching Publications.

Mayer, R. E. (2009). *Multimedia learning* (2nd ed.). Cambridge University Press.

Phillips, J. J., & Phillips, P. P. (2016). *Handbook of training evaluation and measurement methods* (4th ed.). Routledge.

Schmidt, R. W. (1990). The role of consciousness in second language learning. *Applied Linguistics, 11*(2), 129–158. https://doi.org/10.1093/applin/11.2.129

Witt, S. M., & Young, S. J. (2000). Phone-level pronunciation scoring and assessment for interactive language learning. *Speech Communication, 30*(2–3), 95–108. https://doi.org/10.1016/S0167-6393(99)00044-8

European Union. (2016). *Regulation (EU) 2016/679, General Data Protection Regulation*. OJ L 119.

European Union. (2024). *Regulation (EU) 2024/1689, Artificial Intelligence Act*. OJ.

> **Note.** Before deposit, §3.2 should be extended with the 2024–2026 literature on automated speech assessment using language models, and §3.3 with recent work on uptake and corrective feedback in interaction with agents.

---

*© 2026 Ana Eslava-Graterol — MLLDE (Universitat Politècnica de València). TK Coach and "Capi" © Talketika. The CEFR (Council of Europe) is paraphrased and cited, not reproduced; Cambridge, xAPI (ADL/IEEE), IPA and ESCO are cited as standards. Prepared with AI assistance; reviewed and approved by the author, in the spirit of Article 50 of the EU AI Act.*
