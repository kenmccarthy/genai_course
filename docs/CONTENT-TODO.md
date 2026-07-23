# Content to insert before go-live — SETU checklist

The course content now comes from the detailed script. The items below are the
remaining SETU-specific pieces, marked in the course with a dashed
"SETU content to insert" box or `[SETU to confirm]`. Search the codebase for
those to find each spot.

## Responsible AI at SETU (section 5)
- [ ] **Position Statement** — add a link to the full Position Statement on Generative AI (or embed a summary + link).
- [ ] **AI Principles** — confirm the five principles (Human-centred, Responsible, Critical, Inclusive, Innovative) match the official wording; add a link to the Principles document.

## AI at SETU (section 6)
- [ ] **AI Governance Structure graphic** — insert the official diagram (placeholder box is in place).
- [ ] **Guidance resources** — confirm the six resource cards (Position Statement, Staff & Student Guidelines, Assessment Redesign Framework, AI Integration Framework, Exemplars & case studies, Professional development) and add links to each.
- [ ] **AI at SETU website** — add the "start here" hub link and a contact email.

## Completion screen (section 10)
- [ ] **Module 2 (AI Competency)** — add the name and enrolment link.

## Branding (done, but confirm)
- [x] SETU logo wired into top bar (light + dark) and cover hero.
- [x] Slate Grey primary + secondary accent palette applied (Brand Guidelines v1).
- [x] DM Sans (headings) + Inter (body) self-hosted from `assets/fonts/`.
- [ ] Optional: replace extracted PNG logos with official **SVG/EPS** vector files (better for print). Current logos were extracted from the brand-guidelines PDF.
- [ ] Confirm brand hex values in `:root` in `assets/css/styles.css` if any differ.

## Structure note for SETU review
- The outline table listed **Welcome** and **Why AI Matters** as separate sections; the
  narrated script delivers them as one flowing welcome, so they are combined in
  **section 1 (Welcome)**. If you want them split, provide the distinct "Why AI Matters"
  copy and it can become its own section.

## Authored-to-spec content to review
These activities were built to fulfil the script's brief where it described an activity
but didn't provide the exact text — please review for tone/accuracy:
- [ ] **How AI Works → "Spot the hallucination"** — the three sample answers (fabricated citation example).
- [ ] **Strengths & Limitations → "AI or Human?"** — the per-task discussion notes.
- [ ] **Strengths & Limitations → "Would you trust this?"** — the sample AI passage containing a factual error, a fabricated reference, and a biased statement.

## Optional / general
- [ ] AI working group to review sections 1–7 for accuracy and SETU tone.
- [ ] Confirm the ~60-minute total and per-section time estimates after a pilot read-through.
- [ ] Decide whether completion tracking is needed (would require LMS/SCORM hosting).
- [ ] Accessibility sign-off against SETU's WCAG target.
- [ ] Brand note: the course uses light emoji icons (as the script itself does for the role pathway). Confirm this is acceptable, given the Brand Guidelines advise against emojis in *official communications* — or ask and they can be swapped for line icons.
