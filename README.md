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

```
index.html            The whole course (all 9 topics + cover + completion)
assets/css/styles.css  Design system (SETU brand tokens at the top)
assets/js/course.js    Navigation, progress, activities, reflection
assets/img/            (place a logo here — see below)
docs/CONTENT-TODO.md   Checklist of SETU-specific content still to insert
```

## Features

- **Progress bar** that remembers the furthest point reached (saved in the browser).
- **Contents panel** for jumping between topics; collapses to a drawer on mobile.
- **Interactive activity** — "Which of these are AI?" with reveal-and-explain feedback.
- **Animation** — a next-token predictor showing how an LLM builds a sentence.
- **Self-check questions** with instant, explained feedback (no pass/fail gate).
- **Reflection exercise** — autosaved locally, downloadable as a text file.
- Accessible (keyboard nav, skip link, focus states, reduced-motion support),
  responsive, light/dark aware, and printable to PDF.

## Run it locally

Just open `index.html` in a browser. Or serve the folder:

```bash
python3 -m http.server 8000    # then visit http://localhost:8000
```

## Before it goes live — SETU to complete

This build ships with **clearly-marked placeholders** for content only SETU can confirm.
Search the project for `SETU to confirm`, `placeholder__flag`, and see
**`docs/CONTENT-TODO.md`** for the full checklist. In short:

1. **Topic 6 – Responsible AI:** paste the official Position Statement and AI Principles.
2. **Topic 7 – AI at SETU:** real governance, working groups, guidelines, assessment
   framework, support contacts and policy links.
3. **Completion screen:** name of Module 2 and how to enrol.
4. **Branding:** drop the SETU logo into `assets/img/` and swap the `.brand-mark`
   in `index.html`; set official brand colours in the `:root` tokens at the top of
   `assets/css/styles.css`.

## Branding tokens

All colours live as CSS variables at the top of `assets/css/styles.css`
(`--brand`, `--accent`, tints, etc.). Change them there once and the whole course updates.

## Notes

- Progress and reflections are stored in the visitor's own browser (`localStorage`),
  not on any server — nothing personal leaves the device. If SETU needs completion
  tracking for records, that would come from hosting inside the LMS (a possible future
  step; see the delivery-format options discussed at kickoff).
