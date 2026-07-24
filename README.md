# SETU GenAI Programme — Module 1: AI Literacy

A self-paced, ~1-hour web course that is the shared foundation of SETU's three-part
GenAI programme. Aimed at all SETU staff. No maths, no jargon.

**Course 1 of 3** · Learning outcomes, topics, and interactive activities as specified
in the course brief.

## What it is

A **standalone static website** — plain HTML, CSS and JavaScript with **no build step
and no dependencies**. It runs by opening a file in a browser and can be hosted anywhere
(GitHub Pages, the SETU web server, an intranet folder, or an LMS as an embedded/uploaded
package).

## Two ways to distribute — one source

The same `index.html` + `assets/` power **both**:

1. **Standalone website** — host the folder anywhere (GitHub Pages, the SETU web
   server, an intranet). Nothing to build.
2. **SCORM package for your LMS** — run `python3 scorm/build_scorm.py` to produce
   `dist/setu-ai-literacy-scorm-1.2.zip`, then upload it to Moodle/Brightspace/etc.
   The LMS tracks progress, resume position and completion. See **`scorm/README.md`**.

The SCORM adapter (`assets/js/scorm.js`) is inert without an LMS, so the website version
is unaffected and the two never diverge.

```
index.html             The whole course (9 sections + cover + completion)
assets/css/styles.css   Design system (SETU brand tokens at the top)
assets/js/course.js     Navigation, progress, activities, reflection
assets/js/scorm.js      SCORM 1.2 adapter (no-op outside an LMS)
assets/fonts/           Self-hosted DM Sans + Inter (brand fonts) + fonts.css
scorm/                  Build script + packaging docs
dist/                   Built SCORM .zip (regenerate with the build script)
assets/img/             SETU logo assets (light/dark) + favicon
docs/CONTENT-TODO.md    Checklist of SETU-specific content still to insert
```

## Branding

Built to the **SETU Brand Guidelines (v1, May 2022)**:
- **Colour** — Slate Grey `#435465` primary with the secondary accent palette
  (Sea Green, Barrow Blue, Sunset Red, Sunrise Yellow) for interactive and semantic
  states. All tokens live at the top of `assets/css/styles.css`.
- **Typography** — DM Sans (headings) and Inter (body), self-hosted in `assets/fonts/`
  so the course is fully self-contained and works offline.
- **Logo** — master logo in the top bar (with a white variant that swaps in for dark
  mode) and on the cover; the crest symbol as the favicon. Assets were extracted from
  the brand-guidelines PDF; official SVG/EPS files can replace them later.

## Sections

Welcome · Understanding AI · How AI Works · Strengths & Limitations ·
Responsible AI at SETU · AI at SETU · Working Effectively with AI ·
AI in Practice · Reflection — plus a cover and a completion screen. Content is
drawn from the detailed course script.

## Features

- **Progress bar** that remembers the furthest point reached (saved in the browser).
- **Contents panel** for jumping between sections; collapses to a drawer on mobile.
- **Interactive activities**, each drawn from the script:
  - "Which of these use AI?" — select-and-reveal with explanations.
  - Next-token predictor **animation** + "complete the sentence" demo.
  - "Spot the hallucination" self-check with explained feedback.
  - "AI or Human?" task spectrum with discussion notes.
  - "Would you trust this?" — click the flags in an AI answer (factual error,
    fabricated reference, biased statement).
  - "Think like a professional" reveal checklist.
  - Role **pathway** tabs (Teaching, Assessment, Research, Professional Services,
    Leadership, Accessibility) with case studies.
- **Reflection exercise** — autosaved locally, downloadable as a text file.
- Accessible (keyboard nav, skip link, focus states, reduced-motion support),
  responsive, light/dark aware, and printable to PDF.

## Run it locally

Just open `index.html` in a browser. Or serve the folder:

```bash
python3 -m http.server 8000    # then visit http://localhost:8000
```

## Before it goes live — SETU to complete

The narrated content is in place from the script. A few **SETU-specific pieces** remain
as clearly-marked placeholders. Search the project for `SETU to confirm` /
`placeholder__flag`, and see **`docs/CONTENT-TODO.md`** for the full checklist. In short:

1. **Responsible AI at SETU:** links to the Position Statement and AI Principles.
2. **AI at SETU:** the governance-structure graphic, resource links, and the hub link + contact.
3. **Completion screen:** the name of Module 2 (AI Competency) and how to enrol.
4. **Logos (optional):** swap the extracted PNGs for official SVG/EPS vector files for print.

## Branding tokens

All colours live as CSS variables at the top of `assets/css/styles.css`
(`--brand` = Slate Grey, `--accent` = Sea Green, secondary palette, tints, etc.).
Change them there once and the whole course updates. Fonts are defined in
`assets/fonts/fonts.css`.

## Notes

- In the **website** version, progress and reflections are stored in the visitor's own
  browser (`localStorage`) — nothing personal leaves the device.
- In the **SCORM/LMS** version, completion, progress and resume position are reported to
  the LMS for record-keeping (reflection notes still stay on the device). Rebuild the
  package with `python3 scorm/build_scorm.py` after any content edit.
