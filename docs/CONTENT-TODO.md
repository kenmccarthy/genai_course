# Content to insert before go-live — SETU checklist

The course content and interactions are in place. The items below are the remaining
SETU-specific pieces, marked in the course with a dashed "Image / Video / SETU content
to insert" slot or `[SETU to confirm]`. Search the codebase for `placeholder__flag`,
`figure__slot`, `video__slot`, and `SETU to confirm`.

## 1. Images (you are supplying these)
Every slot is a `<figure class="figure">` with a dashed placeholder. To fill one,
replace the inner `<div class="figure__slot">…</div>` with `<img src="assets/img/your-file.jpg"
alt="…">`. Recommended: SETU photography style (shallow depth of field, natural light,
authentic, inclusive). Suggested sizes below (all can be larger; keep the aspect ratio).

| Section | Where | Suggested size / ratio |
|---|---|---|
| Welcome | Banner under the hero | 1600×540 (3:1) |
| Understanding AI | Header (concept diagram) | 1200×675 (16:9) |
| Understanding AI | Closing image after the activity | 1200×675 (16:9) |
| How AI Works | Header illustration | 1200×675 (16:9) |
| How AI Works | “When AI takes things literally” (optional) | 1200×675 (16:9) |
| Strengths & Limitations | Header illustration | 1200×675 (16:9) |
| Responsible AI at SETU | Header illustration | 1200×675 (16:9) |
| AI at SETU | Header illustration | 1200×675 (16:9) |
| Working Effectively | Header illustration | 1200×675 (16:9) |
| AI in Practice | Header illustration | 1200×675 (16:9) |
| Reflection | Reflective image | 1200×675 (16:9) |

## 2. Video — AI at SETU
- [x] **YouTube video wired** — the AI Integration plan overview
  (`https://youtu.be/K0J3JcAN37U`) is embedded inline (privacy-enhanced
  `youtube-nocookie`), with a "watch on YouTube" fallback link for offline/SCORM.
  Note: some LMS content-security policies block external iframes; the fallback link
  covers that. To change the video, edit the `data-video` block in `index.html`.

## 3. Responsible AI at SETU
- [ ] **Position Statement** — add the link (placeholder in place).
- [ ] **AI Principles** — confirm the five principles (Human-centred, Responsible, Critical,
  Inclusive, Innovative) match the official wording, and **confirm the source document**
  (the review asked whether these come from the Staff Guidelines). Add the link.

## 4. AI at SETU
- [ ] **AI Governance Structure graphic** — insert the official diagram (placeholder in place).
- [ ] **Resource links** — add links on the six resource cards.
- [ ] **AI at SETU website** — add the “start here” link and a contact email.

## 5. Completion / certificate
- [ ] **Course 2 (AI Competency)** — add the name and enrolment link (placeholder in the
  “Where next” box).
- [ ] **Certificate wording** (optional) — the certificate reads “SETU GenAI Programme /
  Course 1 — AI Literacy”. If you want a signatory line (e.g. a name/title) or a QR/verify
  note, say so and it can be added. The learner types their own name; the LMS also records
  completion via SCORM.

## 6. Branding (done — confirm)
- [x] Terminology standardised to **courses + sections** (no “module”/“stage”/“hub” as
  structural terms).
- [x] SETU logo, Slate Grey + secondary palette, DM Sans/Inter fonts.
- [ ] Optional: replace the extracted PNG logos with official **SVG/EPS** vector files.

## 7. Review notes (from the feedback doc — addressed, worth a final check)
- Flip cards used for **What AI does well** and the **AI Principles** (tap/click/Enter to flip).
- Consistent **Key message** boxes (yellow “Key message” pill) added across sections, with
  bullet points where useful; the How AI Works key message is now a distinct colour from the
  box above it.
- New activities: Responsible AI **scenario**, Working Effectively **“improve this prompt”**,
  and interactive **case-study reveals** in AI in Practice. Please review these for tone.
- The **five key takeaways** now live in **Reflection** (moved out of “Well done”).
- “Complete the sentence” example changed from “Fish and chips…” to “The early bird catches
  the…”.

## 8. Optional / general
- [ ] AI working group to review all sections for accuracy and SETU tone.
- [x] Emojis replaced with a set of SVG **line icons** (brand-appropriate), per the Brand
  Guidelines note on official communications.
- [ ] Accessibility sign-off against SETU’s WCAG target.
- [ ] After any edit, rebuild the SCORM package: `python3 scorm/build_scorm.py`.
