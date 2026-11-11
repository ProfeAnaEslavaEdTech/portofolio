# Agent instructions — portfolio repo

## ⚠️ DO NOT MODIFY — published academic appendices (frozen)

These are published academic materials. They are **frozen**: do NOT edit, restyle,
rename, move, delete, or "redesign to the model". They are linked from the portfolio
but are **not** part of the Ocean Ink design system and must be left exactly as-is.

- **`metadiscourse-visualization.html`** (this repo) — the interactive data book that is
  the **appendix of the master's thesis (TFM)**, published at
  https://profeanaeslavaedtech.github.io/portofolio/metadiscourse-visualization.html
- **Databook** repo (`ProfeAnaEslavaEdTech/Databook`) — the **TFM** repository. Off-limits.
- **mllde-xapi** repo (`ProfeAnaEslavaEdTech/mllde-xapi`), published at
  https://profeanaeslavaedtech.github.io/mllde-xapi/ — the **appendix of an article being
  published**. Off-limits.
  *Exception decided by Ana (10 Nov 2026):* the MLLDE AI-governance norms live in
  `governance/` of this repo. Work on them only on a branch; merge to `main` only with
  Ana's explicit go-ahead, because `main` is the published appendix.
- **Gamification** repo (`ProfeAnaEslavaEdTech/Gamification`), the *Academic Writing
  Journey* course, published at https://profeanaeslavaedtech.github.io/Gamification/ —
  **part of the TFM**. Off-limits (link to it, never modify or redesign it).

## Everything else

The rest of the portfolio follows the **Ocean Ink hub model** (the hub at
`/portofolio/` is the canonical reference). See the `ocean-ink-design-system` skill:
bilingual EN/ES, light/dark, sober minimal layout, band-palette facet funnel, no emojis.

## Git

Commit with `ProfeAnaEslavaEdTech@users.noreply.github.com` (private email is blocked).

## Audit principle — no claim without its proof (Ana Eslava-Graterol, 10 Nov 2026)

> **Principio de auditoría:** cotejar cada afirmación con los datos es lo que destapó los fallos de TK CoachAI. Si se hubiera aceptado lo que se decía sin comprobarlo, seguiríamos con cifras falsas. Cotejar no es lentitud: es la auditoría. Para la gobernanza, ninguna afirmación se da por buena sin su prueba (IDs de sentencias en el LRS, extracto de código y fecha desde la que se cumple).

How agents working for Ana apply it:
- Treat every "implemented", "done", "fixed" or "verified" from a developer, a vendor, a document or another AI agent as a **claim**, not a fact.
- Accept it only with its three proofs: **(a)** statement IDs in the LRS, **(b)** the code excerpt, **(c)** the date from which it holds. Until then, mark it **pending**.
- Check against **independent data** (the external LRS export), not only against the reporter's own summary or a second model's review.
- Apply it to your own output too: before a document, slide or email states a figure or a fact, check it against the data, and correct it if the data say otherwise.


## Decisions propagate at once (Ana Eslava-Graterol, 10 Nov 2026)

> «Todos los cambios hay que hacerlos actualizados a medida que vamos tomando las decisiones, para que nada quede por fuera y desactualizado.»

How agents working for Ana apply it:
- When Ana takes a decision, update **every** affected document in the same session. That covers norms, specifications, agent cards, the agent registry, the question script, the decision register, the deck and the video script. Then say which ones you changed.
- Never leave yesterday's version of a document contradicting today's decision. Write a new dated version, or mark the old text as replaced and give the date.
- In `mllde-xapi`, the changes still go to a branch only (see the exception above).
- **Errors already corrected stay off the correction list** (Ana, 11 Nov 2026). An error counts as corrected when the independent LRS data show it no longer happens, or when it has its three proofs. If the old data or screen still affect learners or teachers today, it is not corrected.

## Role-invariance principle (Ana Eslava-Graterol, 10 Nov 2026)

> Ningún agente decide, y todos se apegan a su rol, sea cual sea el modelo, se llame como se llame, y sea cual sea la temperatura que aplique el sistema.

When you design or review an AI agent for Ana:
- **Code and tests enforce the role,** not model parameters: a validated output schema, ids from the base, the common block, the R-ID checks A1–A4 and a repeated-input stability test.
- **Record the exact model identifier,** to audit it, not to trust it.
- **A change of model is a new version,** and it repeats the tests.
