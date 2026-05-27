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
- Then: Up straight away / Negotiated within 10 min / Negotiated took longer / Just lay there
Bonus: Wabi / Sunpo / Ma — optional, logged separately

## Tracking — Body tab
Logged post-gym using Yesterday toggle (so logged morning after)
- Bloat: None / Mild / Bloated
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

## Phase 2 — not started
Focus: wake-up anchor
Trigger: Phase 2 readiness graph turns green in app.
What we know already: bed sheet folding already happens naturally. 10 minute negotiation window being practised. Wake time data from Phase 1 will show actual pattern.
Key design principle: not about waking earlier. About having one consistent physical anchor that fires at whatever time you wake — 7am or 10:30am, same trigger.
Wake data collected in Phase 1 will inform exact design of Phase 2 system.
Two rest types distinction (intentional vs reactive) becomes relevant here — Phase 1 logs wake time and negotiation pattern which gives this data without needing separate rest categorisation.

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
