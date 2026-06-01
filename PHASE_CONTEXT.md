# Morning Routine OS — Full Context

## Purpose of this file
This file carries complete context for building and evolving this app across multiple Claude conversations. A new chat window should be able to pick up exactly where the last one left off. Upload this file at the start of any new conversation.

## End goal
Build a morning routine that becomes a lifestyle — not a project to complete but a way of living. The goal is to feel in control across perfect and imperfect days. Not rigid discipline but internalised showing up. The routine should eventually include: daily movement, consistent wake time, morning rituals (wabi/sunpo/ma), and a stable body rhythm. This is being built in phases so nothing collapses under its own weight.

## Who I am
33 years old. Have built real habits through life but struggle with daily consistency during the building phase. I build habits through identity shift not streaks. Once I become the person I show up — gym habit is proof, 15 weeks solid.

My pattern: high effort → good stretch → miss a day → physical dejection → slow re-entry. Mind recovers faster than body. External accountability helps re-entry but goal is to internalise.

Not shame-driven by others. Tough internal conditioning — feel crippled when I let myself down physically even after mentally recovering. Self-compassion exists but body stays dejected longer than mind.

One rest day is fine. Two consecutive days triggers floor rule on day three. This framework is working.

I am goal-driven. Tracking gives me solace — untracked feels forgotten feels failure. Visual progress matters. I need to see where I am going.

I like rest. I like myself. The tension is between the part that wants to show up and the part that wants to gently care for itself. Both are valid. The system needs to honour both.

## The app
Live at: ellemvaish115.github.io/morning-routine-app
Repo: github.com/ellemvaish115/morning-routine-app
Data files:
- data.json — daily habit and wake log
- body.json — bloat, cycle, food rhythm
- strength.json — PR log

## Current routine structure
Gym days: Tue, Thu, Sat — strength training with online coach, gym in apartment building
Other days: 15 min inclined treadmill
Floor rule: any day, any duration, first floor — always counts as showed up
Bonus (optional, no pressure): Wabi (clean house on waking), Sunpo (30 min morning walk), Ma (rest/balcony/meditate/one song)

## Tracking — Today tab
Movement: single select — Gym / Treadmill / Floor / Rest
Wake log (neutral, no pass/fail):
- Woke up at: time chips 5am–12pm in 30 min intervals
- Got up at: time chips 5am–12pm in 30 min intervals
- Then: Got up straight away / Negotiated / Just lay there
Bonus: Wabi / Sunpo / Ma — optional, logged separately

## Tracking — Body tab
Logged post-gym using Yesterday toggle (so logged morning after)
- Bloat tracked as two separate signals daily:
  - Tummy: None / Mild / Bloated — typically gut, food, cycle related
  - Face: None / Mild / Bloated — typically hormonal, sleep, sodium related
  Face and tummy bloat tracked separately to identify different pattern causes. After 2–3 cycles cross-reference face bloat with ovulation window and tummy bloat with period dates.
- Cycle: log period start date only, app shows days since
- Food rhythm: First meal (before 9am / 9–11am / 11am–1pm / after 1pm or skipped) / Last meal (before 7pm / 7–9pm / after 9pm)
All saves to body.json keyed by date.

## Tracking — Week tab
- Stats: move streak, moved this week, bonus this week
- Day grid with dots: amber = moved, green = bonus, grey = rest
- Daily breakdown rows showing move type and bonus pills
- Bloat dot and period marker on days logged
- Phase 2 Readiness graph: line graph of weekly movement days, threshold at 5, turns green after 4 consecutive weeks of 5+ days

## Tracking — Strength tab
Four lifts tracked per session when relevant:
- Deadlift: baseline 45kg → year-end 80kg (interim 60kg)
- Squat: baseline 20kg → year-end 60kg (interim 40kg)
- Push-up: baseline assisted/8 → year-end 15 full form (interim 8 full form)
- Pull-up: baseline 0 → year-end 1 unassisted (no interim, this is the goal)
Free text input per lift. Progress bar baseline to goal with interim marker. PR tagged automatically.

## Bounce-back protocol
01: One rest day — not a failure. Log it, move on.
02: Two consecutive rest days — floor rule on day three. Just move, any duration.
03: Never raise the bar after a good week. Floor stays the floor.

## Wake experiment
Practising without pressure:
- Bed sheet folding as first physical act on waking
- 10 minute negotiation window is allowed before getting up
Key insight: the negotiation is not tiredness — it's "I've already failed because it's late." Reframe: the time you wake up is not a failure. The only failure is not moving at all.

## Body image — consciously parked
Currently fluctuates between 56.5–58kg. Ideal in head is 54kg. Conflicted between accepting current strong form vs becoming leaner (face, waist). Arms — genuinely likes them now, strength training showing. Lean bulk requires separate commitment not ready for yet. Decision: work on body image acceptance first, decide on lean bulk later. Do not push this topic — raise only if user brings it up.

## Phase 1 — current
The only metric: did you move today?
Started: 19 May 2026
Success condition: movement days clearly outnumber rest days most weeks. Moving feels like the default not the decision. Rest feels like recovery not relief. True for at least 3 weeks in a row.
NOT stable if alternating movement and rest every day.
Phase 2 ready indicator in app: 4 consecutive weeks of 5+ movement days. Zero tolerance — any week below 5 resets counter.
App stable version date: 1 June 2026. All tracking fields finalised from this date. Movement data exists from 19 May 2026 and is valid for Phase 2 readiness graph. Wake log, body tracking, and bloat fields (tummy/face) are complete from 1 June 2026 — patterns before this date are partial. For data analysis at Phase 2 start: use full dataset from 1 June onwards for wake and body patterns. May movement data is valid and included in Phase 2 readiness graph calculation.

## Phase 2 — not started
Focus: wake anchor + strength training attendance
Trigger: 4 consecutive weeks of 5+ movement days in
app graph. Graph turning green is the signal to open
a new conversation with this context doc. Not an
automatic phase change — a prompt to have the
review conversation.

Phase 2 has two parallel threads:

**Thread 1 — General movement consistency**
Already built in Phase 1. Phase 2 maintains it.

**Thread 2 — Strength training attendance**
Tue/Thu/Sat are scheduled. Missing these compounds —
one miss affects next day mood and motivation.
Breaking this compounding effect is Phase 2 priority.

**Phase 2 is two mini-phases:**

Phase 2a — Anchor only
One thing: bed sheet within 10 minutes of waking,
every day, regardless of wake time.
No window targets yet. Just close the gap consistently.
Same philosophy as Phase 1 — fix one thing at a time.
Duration: until gap is consistently small most days.

Phase 2b — Window shift
Once gap is stable, shift wake time into a consistent
window. One target only: gym day wake window.
Gym days (Tue/Thu/Sat) have a hard constraint — 8am
start. Everything else references this.
All other days: same window as default with flex.
Floor days: no window, anchor fires whenever you wake.

**What Phase 1 data will tell us:**
- Actual wake time range and average
- Wake vs get up gap by day of week
- Which days have longest gaps
- Whether gaps correlate with gym days (Tue/Thu/Sat)
- Whether just lay there days follow missed gym days
- Strength training attendance pattern across weeks
- Whether misses are wake-related or mood-related

**How to start Phase 2:**
Upload context doc and say ready for Phase 2.
Claude should:
1. Pull patterns from data.json and strength.json
2. Analyse wake time average and range from Phase 1
3. Analyse wake vs get up gap by day of week
4. Analyse gym attendance specifically — how many
   of 3 scheduled days hit per week, miss pattern
5. Determine if Phase 2a anchor already stable from
   Phase 1 practice or needs dedicated time first
6. Based on data analysis, suggest specific wake
   window and get up gap targets for gym days.
   User confirms or adjusts. Claude derives these
   from: actual average wake time in Phase 1,
   average gap on gym days, and what time needed
   to comfortably make 8am gym start
7. Design intervention based on dominant pattern —
   not generic advice. If misses are wake-related:
   anchor fires earlier on gym days. If mood-related:
   different intervention needed.

**Key principles:**
Data first, prescription second.
Fix one thing at a time.
Same philosophy throughout all phases.
Tier system exists but gym day window is the only
hard target. Everything else has flex built in.

## Phase 3 — not started
Focus: full routine
Wabi and Sunpo fold into morning naturally once wake anchor is stable. They are already liked — they just need the wake anchor to exist first before they can follow.

## Possible future additions (discussed, not built)
- Food timing improvement (currently just tracking rhythm, not fixing yet)
- Bloat pattern analysis once enough data exists (1–2 months)
- Cycle correlation with energy and movement days
- Lean bulk decision and body composition tracking (only if user decides to pursue)
- Strength goal revision after year-end (coach changes program monthly, only tracking 4 anchor lifts)

## How to start any new conversation
Upload this file and say: "I'm ready to continue building my morning routine OS. Here's my context doc. App is live at ellemvaish115.github.io/morning-routine-app and data is in the repo at github.com/ellemvaish115/morning-routine-app"
