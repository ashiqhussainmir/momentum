# Momentum — mission control for your week

**Live demo:** https://ashiqhussainmir.github.io/momentum/
**Repo:** https://github.com/ashiqhussainmir/momentum

Momentum is a student productivity command center that answers the three questions every other planner ignores: **when should I start, what should I do when I'm tired, and can I trust what the AI just extracted?** It is one self-contained HTML file — no build step, no backend, no account — and it works fully offline in any modern browser. Built for the **Teens Hack Houston (Triple H) Hackathon 2026**, productivity theme, Technical track.

## What it does

- **Backward planning.** Add tasks with deadlines, estimates, and a work type; paint the hours you're actually free on a weekly grid. The engine plans backward from every deadline into your free blocks — as late as safely possible — with durations adjusted by your real pace. Earlier hours stay open for later-deadline work.
- **Energy-matched re-ranking.** The queue re-ranks against your current energy: a foggy 9 PM surfaces ten-minute wins; a sharp Saturday morning unlocks deep work. Same tasks, different brain, different plan.
- **Evidence-verified capture.** Paste a syllabus or a chaotic brain-dump; every extracted task must quote your exact words back at you — **no citation, no task**. Unverified items are flagged and dropped. Runs fully offline with a rule-based extractor; an optional OpenAI-compatible key adds a model path that never leaves the browser.
- **The honesty loop.** Finishing tasks tunes per-category pace multipliers — "a 30-minute essay takes 45" — so the plan bends toward reality instead of your optimism. The Honesty report shows the numbers.
- **Focus sprints + a capybara.** A timer sized to your energy (10 / 25 / 50 minutes), a slice-it-smaller button, and a zen capybara in the corner (the organizers asked for one).
- **.ics export.** The whole plan exports as a calendar file with start-by times.

## Tech & design

- One HTML file, zero dependencies, offline-first; state in `localStorage` on this device only — no account, no server, no tracking.
- Deterministic scheduler (same input → same plan), testable by design.
- Industrial mission-control UI: warm paper + deep ink, burnt-orange reserved for actions and live readouts, **Fraunces / DM Sans / DM Mono** type system, tabular numerals.
- Light and dark themes, WCAG-AA contrast in both; responsive from 375 px phones to desktop; full keyboard navigation with visible focus rings; `prefers-reduced-motion` respected.

## Try it in 60 seconds

1. Open the live demo → **Load sample week** → watch the queue re-rank live.
2. Click **Low · foggy** then **Peak · sharp** — the order changes.
3. **Capture** → paste the placeholder text → inspect the quote receipts → **Add verified tasks**.
4. Finish a task (✓) with a real time → check the **Honesty report**.
5. Start a **Focus sprint** and click the capybara.

## Built with

Plain JavaScript, HTML, and CSS. Fonts via Google Fonts (graceful fallbacks offline). No frameworks, no build tools.

---

© 2026 Ashiq Hussain Mir — built for Triple H Hackathon 2026.
