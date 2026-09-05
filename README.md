# portofolio

My EdTech portfolio.

## Doctoral Project — MLLDE

**[`doctorado.html`](doctorado.html)** — the doctoral project page (bilingual ES/EN, light and dark
themes) for the thesis proposal *"MLLDE — Mobile Language Learning Design Environment: a method for
integrating LLM tutors and AI literacy into CEFR curriculum design"* (PhD Programme in Applied
Linguistics, Department of Applied Linguistics, Universitat Politècnica de València).

The full file lives under [`doctorado/`](doctorado/):

| Path | Contents |
|------|----------|
| `doctorado/README.md` | Guide to the file — how the CV maps to the programme's scoring rubric and what is still pending. |
| `doctorado/01-propuesta/propuesta-doctoral-MLLDE-ES.md` | Doctoral proposal in Spanish — state of the art, research gap, questions, objectives, hypotheses, design-based methodology in three cycles, four-year timeline, ethics and APA 7 references. |
| `doctorado/01-propuesta/doctoral-research-proposal-MLLDE-EN.md` | The same proposal in English. |
| `doctorado/02-cv-baremo/cv-doctorado-baremo-ES.md` | CV structured to the call's rubric — academic record 70% + six merits at 5% each — with `DOC-nn` codes to the supporting evidence. |
| `doctorado/02-cv-baremo/cv-doctorado-baremo-EN.md` | The same CV in English. |
| `doctorado/03-anexos/indice-documentos-acreditativos.md` | Bilingual cover-index for the single supporting-evidence PDF (DOC-01 → DOC-23). |

---

## Interactive Corpus Data Book

**`metadiscourse-visualization.html`** — an interactive data book for the master's
thesis *"Disciplinary Variation in Metadiscourse Use across Master's Thesis
Abstracts"* (Prof. Mª Luisa Carrió-Pastor & Prof. Ana Eslava-Graterol, Department
of Applied Linguistics, Universitat Politècnica de València).

It renders the corpus results live from the source workbook:

- **Cover page** with the thesis identity and headline metrics (6 subcorpora ·
  180 abstracts · 18,000 words · 920 markers · 4,049 TFMs in the sampling frame).
- **Animated overview video** of the cross-disciplinary findings.
- **Lexical profile** of each subcorpus (words, types, tokens, TTR).
- **Metadiscourse markers** across all six disciplines — textual vs interpersonal,
  ten Hyland (2005) categories, toggle raw occurrences ↔ frequency per 1,000
  tokens, filter by marker type.
- **Per-discipline deep dive** — category profile, subcategory breakdown and the
  most frequent markers in each subcorpus.
- **Sampling population** by access status (open / closed).
- **Method notes & limitations**, plus a download of the full Excel workbook.

Every chart has a data-table view and a colour-vision-deficiency-validated palette,
works in light and dark mode, and is fully self-contained (Chart.js vendored under
`vendor/`; no external dependencies).

### Files

| Path | Contents |
|------|----------|
| `metadiscourse-visualization.html` | The interactive data book (self-contained). |
| `assets/appendix-corpus-metadata-and-results.xlsx` | Source workbook (18 sheets). |
| `assets/corpus-intro-video.mp4` | Animated results overview. |
| `vendor/chart.umd.min.js` | Chart.js 4.4.0 (vendored for offline/GitHub Pages use). |
