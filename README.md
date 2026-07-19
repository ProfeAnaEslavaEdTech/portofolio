# portofolio

My EdTech portfolio.

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
