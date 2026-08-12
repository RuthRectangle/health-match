# health-match — Guided Intake Prototype

A single-file, click-through prototype of a **symptom-led guided entry** flow, sitting alongside specialty search rather than replacing it. Built as a static `index.html` (no build step, no backend) to make the "prepared patient" concept tangible for stakeholder review.

**Live file:** `index.html` — open directly in a browser, or serve statically (e.g. GitHub Pages).

## What it demonstrates

A patient who doesn't know which specialist they need can describe what's going on in their own words instead of searching by specialty. The prototype walks through:

1. **Entry** — existing specialty/name search, plus a second, equally visible path: "Tell us what's going on."
2. **Tell us** — free-text symptom description in the patient's own words (explicitly framed as *not* a diagnosis).
3. **Safety check** — a simple red-flag keyword scan (e.g. chest pain, can't breathe, suicidal ideation) that interrupts the flow with emergency guidance (999/A&E) before any matching logic runs.
4. **Clarify** — three quick chip-based questions: affected area, duration, and preferred consultation language — used for sub-specialty and language matching, not just a specialty label.
5. **Recommendation** — a suggested specialty with a plain-English "why," a matched shortlist of doctors, and an explicit override ("this isn't right — let me choose a different specialty") so the patient stays in control.
6. **Format** — a suggested consultation format (video, in person, or phone), defaulting to video as "often enough for an initial assessment."
7. **Confirmation** — booking summary plus a thumbs up/down confidence check, framed as the cheapest instrumentable version of a "did we match you right?" signal.

## Product reasoning built into the demo

Each screen has a **"Show product reasoning"** toggle (bottom of screen) that surfaces the initiative/KR it maps to and the design rationale — useful for walking a stakeholder through the *why*, not just the *what*, without leaving the prototype.

## Status

Prototype only — front-end mockup with hardcoded doctor data and keyword-based safety detection. Not connected to any real backend data, matching logic, or booking system.
