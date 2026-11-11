# Session Notes — 2026-11-11

## Decisiones tomadas hoy

### WCAG 2.2 AA — 3 correcciones aplicadas y mergeadas

#### Corrección 1 — 2.4.1 Bypass Blocks (Nivel A) ✅
- Skip link añadido como primer elemento enfocable del `<body>`
- CSS: `position:absolute; top:-100%` → visible solo en foco (`:focus { top:0 }`)

#### Corrección 2 — 4.1.3 Status Messages (Nivel AA) ✅
- `aria-live="polite" aria-atomic="true"` añadido a `#panelHead`
- Los cambios dinámicos de texto ahora se anuncian a VoiceOver/NVDA

#### Corrección 3 — 1.3.1 Info and Relationships (Nivel A) ✅
- `<h3>` dentro de `<button role="tab">` reemplazado por `<span class="sbtn-label">`
- HTML semánticamente válido; estilos visuales mantenidos con CSS

### Artefactos publicados
- **Informe de auditoría WCAG** (bilingüe ES/EN) con sección "Cambios Realizados"
  - `https://claude.ai/artifact/Azdb88FPvvWDoxNKAUdQKZ`
- **Checklist WCAG 2.2 AA interactivo** (50 criterios A+AA, localStorage, exportar CSV)
  - `https://claude.ai/artifact/A2otBUyujNmQribaW2B4ec`
  - ⚠ Exportar CSV bloqueado en sandbox del artifact viewer (capability `downloads` pendiente)

## PRs cerrados hoy
- **#44** — fix: WCAG 2.2 AA conformance — skip link, aria-live, heading-in-button → mergeado a main (SHA df8ba71)

## Estado actual de main
- Portfolio en `https://profeanaeslavaedtech.github.io/portofolio/` conforme WCAG 2.2 AA para las 3 correcciones
- Declaración: **parcialmente conforme** (2.4.11 Focus Not Obscured pendiente verificación live)

## Pendiente / Para mañana
- Verificar 2.4.11 Focus Not Obscured live (header sticky en producción)
- Posible: habilitar exportación CSV en checklist (capability `downloads`)
- Posible: añadir página pública de declaración de conformidad WCAG
- Posible: audit completo de todas las páginas del portfolio

## Restricciones de marca (siempre activas)
- **Talketika** SIN acento — nunca Talkétika
- Siempre "for Talketika (app owner; software by Orkelia)"
- **"Measure, Not Decide"** — siempre en inglés en ambas versiones
- TK CoachAI es de Talketika, NO proyecto propio de Ana
- MLLDE © Ana Eslava-Graterol. Copyright registration in progress.
- Antonio Estévez Funes — atribución formativa únicamente
