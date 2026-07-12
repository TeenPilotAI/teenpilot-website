# CLAUDE.md — TeenPilot Marketing Website

Orientation for any Claude session working in this repo. Read this first.

## What this repo is

This is the **marketing website only** — currently live at
`teenpilot-website.vercel.app` (not yet on the custom domain).

- The **app** is a **separate repo** (`TeenPilot`), live at `app.teenpilot.co.nz`.
  Do not confuse the two. Changes here are website/copy/marketing, not product.

## Product context

- **TeenPilot** is an AI co-pilot for **NZ secondary school students (minors)** —
  across their whole life: school, sport, work, social, wellbeing. **Safe-first.**
- Founder: **Hadleigh** (Agentec Ltd, Auckland), building with his son **Wyan**
  (14, co-creator and lead tester).
- This is a **product for minors** → safety, privacy, and the **accuracy of public
  claims** matter a lot. Treat every public-facing claim with that in mind.

## Strategy (what the site shows)

- The website shows the **FULL vision** — everything TeenPilot will provide.
- We build everything **before** public launch on the custom domain. The app
  takes **no payments**, and paid/messaging functions **aren't usable yet**.
- So features **stay visible** — but **child-safety and legal/compliance claims
  must be framed as "coming / built to," NOT present-tense guarantees.**
  - ✅ "built to keep teens safe", "designed to…", "coming soon"
  - ❌ "we keep your teen safe", "fully compliant", present-tense promises
- **Tier cards = launch build spec (build-first).** The four **Plans** cards
  (`#pricing`) advertise the full launch line-up, framed as **"arrives at
  launch"** — a commitment we control, not a present-tense claim (paid plans
  aren't purchasable until Stripe is live). **Card ↔ build parity:** if a
  feature is cut from the build, cut it from the card **before launch**. Full
  spec + permanently-excluded list → **`ROADMAP.md`**.

## Merge rule (governance)

- You **MAY merge yourself**: docs / copy / cosmetic / low-stakes,
  easily-reversible changes.
- **Open a PR and STOP** (Hadleigh merges): anything touching **deploy/build
  config** (`vercel.json`, domains), or anything **irreversible**.
- A **mixed PR** = higher-stakes bucket = **his**.
- **Unsure = default to his and ask.**

## Working style

- **Investigate read-only first.** Show the plan / specific changes **before
  editing**. **Don't commit until confirmed** (except pre-authorised docs like
  this file).
- Responses: **concise** — bullets, to the point, full detail, minimal padding.
- Branch: develop on the session's designated `claude/*` branch; never push to a
  different branch without explicit permission.

## Repo facts (technical)

- **Static, hand-written single-page site.** No framework, no build step, no
  package manager.
  - `index.html` — the entire site (HTML + inline `<style>` + inline `<script>`).
  - `audio/` — voice sample `.mp3`s (aria, blockbrain, coach, copilot, hoshi,
    luna, neo, rex).
- **Tech:** vanilla HTML/CSS/JS; Google Fonts (`Syne` display, `DM Sans` body);
  Tabler icons webfont via CDN. Dark theme, accent green `#3dff8f`
  (CSS variables in `:root`).
- **Hosting:** Vercel (static) → `teenpilot-website.vercel.app`.
- **Integrations:** Supabase (waitlist DB — e.g. boarding-pass signups).
- **Editing:** because it's one large file, prefer targeted edits; keep the
  existing CSS-variable system, naming, and section structure consistent.
