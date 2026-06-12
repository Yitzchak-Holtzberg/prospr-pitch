# Prospr Pitch Pages — Design Spec (2026-06-11)

## Goal
Win the commission to rebuild Prospr (Flutter + Google Sheets v1) as a web + mobile
budget planner designed for neurodivergent users. Deliverable for this phase: a static
multi-tab pitch site published on GitHub Pages, showing key screens in desktop and
mobile form.

## Story
Prospr reimagined: same planning brain as v1, redesigned for how ND brains work.
Broad ND umbrella (ADHD, autism, dyscalculia, anxiety) as the narrative; simple
defaults as the near-term scope. Hero concept: **buckets with an allowed-spend
number** — one number you can trust, no running math, no shame states (an overspent
bucket goes calm grey "resting", never red — deliberate contrast with v1's
traffic-light red).

## Decisions (validated with stakeholder)
- **Visual system:** Material 3 Expressive, "Warm Paper" palette — cream #faf6ee bg,
  sage #4f6b4a primary, terracotta #b3704c action, muted containers; Material
  Symbols Rounded icons; pill buttons, large radii, generous spacing.
- **Mobile home:** Bucket Grid — "safe to spend" hero card + 2-up bucket tiles.
- **Desktop shell:** M3 navigation rail + dashboard (hero, 4-up tiles, recent activity).
- **Login:** Minimal Calm — two buttons, one tagline, passwordless-first
  (email link / Google / Apple).
- **Budget screens in pitch:** bucket detail (allowed spend, history, one simple rule)
  and payday allocation wizard (one decision at a time).

## Pages (tabs)
1. `index.html` — cover/manifesto: ND design principles framing the deck
2. `login.html` — desktop + phone frames
3. `home.html` — desktop dashboard + phone bucket grid
4. `bucket.html` — bucket detail
5. `allocate.html` — payday wizard

Each screen page includes a short "why this works for ND users" rationale strip.

## Tech
Plain static HTML/CSS (one shared stylesheet), no framework, no JS beyond trivial
nav state. Hosted on GitHub Pages from a public repo. Fonts: Fraunces (display) +
Plus Jakarta Sans (body) + Material Symbols Rounded.

## Out of scope
The actual app build (web + mobile), real auth, any backend.
