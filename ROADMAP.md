# TeenPilot Website — Launch Build Spec (ROADMAP)

Governance record. Ruling by **Hadleigh, 2026-07-12**. Stands until changed by him.

## The rule — card ↔ build parity

The strategy is **build-first**: the app launches only when **every feature
advertised on the site is real**. Therefore:

- The **four tier cards** in the website's **Plans** section
  (`index.html` → `#pricing`) **ARE the launch build spec.**
- **"Arrives at launch" is a commitment we control — not a present-tense
  claim.** Paid plans are not purchasable until **Stripe is live**.
- **If a feature is cut from the build, it MUST be cut from the card BEFORE
  launch.** No card may advertise a feature that won't ship at launch.
- The canonical product ROADMAP (app repo `TeenPilot`) should mirror this list —
  keep the two in sync.

## The launch spec (as advertised today — keep in lock-step with the build)

**Free — "Get organised" — $0 · available today**
- Co-Pilot chat (fast AI, daily allowance)
- Full life calendar — school, sport, work, activities, holidays
- Squad chat, DMs & family groups — all moderated
- Photo & voice messages (safety-checked)
- Parent portal link · school directory · weather
- Sync to Google & Apple calendar

**Student Pro — "Your study co-pilot" — $14.99/mo · at launch**
- Smarter AI (Sonnet) + a bigger daily allowance
- Snap worksheets & exams — photo help from Co-Pilot
- Study plans & practice questions
- Create group & family events straight from chat

**Advanced — "The AI that plans ahead" — $29.99/mo · at launch**
- Smart routing — best model per task, incl. Opus 4.8 for the hard stuff
- Morning Agent — your day briefed at 7am, before school
- Predictive alerts — busy-week warnings before they bite
- Auto study scheduler — study blocks placed around sport & work
- Transport concierge — live routes, times & directions
- Co-Pilot reminders & wake-up nudges (push)

**Premium — "Everything, remembered" — $49.99/mo · at launch**
- Opus-first for deep work + the highest allowance
- Voice quiz mode — revise out loud with your Co-Pilot
- Long-term memory — Co-Pilot knows your subjects & weak spots
- All avatars & priority voices
- Early access to new features

## Excluded — do NOT restore to the site
group video · TeenPilot Academy · absence email · teacher / school-as-customer
claims · Agentec / Oracle / "enterprise-grade" / SOC-2 fossils · a public launch
date (until Stripe is live).

## Notes
- Model names (**Sonnet, Opus 4.8**) are intentionally public under this framing;
  the earlier "remove all model names" pass is **superseded for the tier cards**.
- Marketing screenshots load from `app.teenpilot.co.nz/marketing/*.png` via
  self-healing device frames (styled placeholder until the assets deploy).
