# Content to insert before go-live — SETU checklist

Everything below is marked in the course with a dashed "SETU content to insert" box
or the text `[SETU to confirm]`. Search the codebase for those to find each spot.

## Topic 6 — Responsible AI (`index.html`, section "Responsible AI")
- [ ] **AI Position Statement** — paste official text or a summary + link to the full document.
- [ ] **AI Principles** — replace the four scaffold principles with SETU's actual principles.
  - The scaffold currently shows: Human oversight · Transparency · Academic integrity · Critical thinking.
- [ ] Confirm the closing "Responsibility stays with you" callout matches SETU's tone.

## Topic 7 — AI at SETU (`index.html`, section "AI at SETU")
Replace each card's `[SETU to confirm]` text and add real links:
- [ ] **Governance** — committee(s) and reporting lines overseeing AI.
- [ ] **Working groups** — named group(s) and how staff get involved.
- [ ] **Guidelines** — staff do's/don'ts + link to current guidance.
- [ ] **Assessment framework** — how AI is handled in assessment + link.
- [ ] **Support** — who to contact, training on offer, approved/supported tools.
- [ ] **Policies** — data protection, IP, academic integrity + links.
- [ ] **"Where to go next"** callout — the single best "start here" link + a contact email.

## Completion screen (`index.html`, final section)
- [ ] Name of **Module 2** and how to enrol / the link.

## Branding
- [ ] Add SETU logo image to `assets/img/` and replace the `.brand-mark` div in `index.html`.
- [ ] Set official brand hex values in `:root` in `assets/css/styles.css`
      (`--brand`, `--brand-strong`, `--brand-tint`, `--accent`, `--accent-tint`).
- [ ] Confirm dark-mode brand values in the `@media (prefers-color-scheme: dark)` block.

## Optional / review
- [ ] Have the AI working group review Topics 2–5 for accuracy and SETU tone.
- [ ] Confirm the "~60 min" and per-topic time estimates feel right after a pilot read-through.
- [ ] Decide whether completion tracking is needed (would require LMS hosting).
- [ ] Accessibility sign-off against SETU's WCAG target.
