# Handoff: Phase 2 (Discovery), persona → user journey
*Written 2026-11-21 at the end of the competitor + persona session. Replaces the Phase 1 → 2 handoff.*

## Where we are
- **Phase 0 (Setup)** and **Phase 1 (Concept)** are done; brief v2 is approved.
- **Phase 2 (Discovery)** so far:
  - ✅ Habit-tracker complaints → `research/user-complaints.md`
  - ✅ Self-interview (key assumption test) → `research/my-past-attempts.md` (+ addendum with 2026-11-21 answers)
  - ✅ Artist's Way practitioner research → `research/artists-way-practitioners.md`
  - ✅ **Competitor analysis** → `research/competitors.md` (verified against live App Store pages; all candidates accepted)
  - 🟡 **Persona** → `research/persona.md` draft v3 (reviewed independently, then updated with my answers). **8 design candidates in it need decisions**, see below.
- The project now lives in the GitHub repo `irinaph/Artist-s`, branch `claude/intelligent-faraday-scp7sh`, with the folder structure the docs refer to.

## Read these first
1. `CLAUDE.md`: your role (PM), scope rule, copyright rule, persona role-play rule
2. `checklist.md`: the task list
3. `01-concept-brief.md`: concept, MVP scope, positioning
4. `project-plan.md`: every decision with its reason
5. `research/persona.md`: the primary persona (me), with evidence tags and open questions
6. `research/competitors.md` and `ideas.md` as needed

## Decided this session (don't reopen)
- **Positioning:** "your pages stay yours: nothing is read unless you choose." Patterns come from my own notes in v1.
- **Artist date** gets an optional **"what came out of it?"** note (text only) in the MVP.
- **AI handwriting scan** parked for later, with conditions (opt-in, after week 8, pages I pick) in `ideas.md`.
- Mobbin references for Phase 3; the name stays **Artist's Sketchbook**.

## Waiting for my decision (persona candidates, `research/persona.md`)
1. **Log late without penalty**, including yesterday (new scope). Sub-question: does the capture ask for the mood *while writing* or *now*?
2. **Remembering to open the app:** a cue on the paper side (card in the notebook) + home-screen shortcut; reminders stay parked.
3. **Medium-neutral capture:** theme = what the pages were about; idea = a creative idea; both free text.
5. **Heavy day → "what's clearer now?"**: unload first, then invite one idea (adjusts the decided "one constructive next step").
6. **Pattern nudges** (new scope): weekly patterns in the day-7 check-in (small); rule-based "new pattern" card inside the app from week 3, no AI, no push (moderate).
7. **Bulgarian and English notes**, with manual merging of synonym themes; Cyrillic-ready fonts. UI language still open.
8. **Irregular writing is normal** (reinforces no streaks / comeback).
- *(4, linking patterns to my creative goal, is parked.)*

**PM recommendation also pending:** I'm not writing pages regularly now, so there is no real data. Try a **paper prototype of the capture** for 1–2 weeks: after each page session, write mood · 1–2 themes · one idea in the notebook margin. It produces real data for the pattern view and tests the quit risks (writing for the tag, patterns saying nothing new) before anything is built.

## Next tasks (Phase 2)
1. Decide the persona candidates above; log them in `project-plan.md`.
2. Optional second archetype (time-starved parent): write or skip.
3. **User journey with mental model** → `research/journey.md`: per step, what happened, what was expected, what she thinks, what she feels. Use the persona's "Through the 12 weeks" strip, quit risks and test scenarios. Weeks 6–12 have no evidence: mark them as assumptions.
4. Persona walkthrough on Mobbin, fresh-eyes review (5 subagents), scope the MVP, handoff to Design.

## Environment notes
- **Mobbin connector works.**
- Web pages: the environment allows `apps.apple.com`, `morningpages.app`, `750words.com`, `www.literati.tools`. The page-reading helper ignores this list, so fetch with `curl` instead. 750words.com blocks automated visits (403).

## First prompt for the new session
> Read HANDOFF.md, then CLAUDE.md, and tell me where we are. Then walk me through the persona's design candidates one by one so I can decide them, and after that start the user journey.
