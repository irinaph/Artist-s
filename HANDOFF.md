# Handoff: Phase 2 (Discovery), user stories → fresh-eyes review
*Written 2026-11-27 at the end of the persona-decisions + journey + user-stories session. Replaces the 2026-11-21 handoff.*

## Where we are
- **Phase 0 (Setup)** and **Phase 1 (Concept)** are done; brief v2 approved (and updated with every decision below).
- **Phase 2 (Discovery):**
  - ✅ Habit-tracker complaints, self-interview, practitioner research, competitor analysis
  - ✅ **Persona** → `research/persona.md` v4: all design candidates decided; two facts confirmed (writes in the kitchen before everyone wakes; has kids)
  - 🟡 **User journey** → `research/journey.md` v2: 11 steps, persona role-play of the five hardest moments folded in (findings R1–R7), journey candidates decided
  - 🟡 **User stories** → `research/user-stories.md` v1: 25 stories in 7 epics with acceptance criteria; **4 open questions** at the end
- **Git:** work lives on branch `claude/lucid-ptolemy-qz9kv3` (it contains everything from `claude/intelligent-faraday-scp7sh`). **`main` is behind** and still has the Phase 1 handoff; merge when I decide.

## Read these first
1. `CLAUDE.md`: PM role, scope rule, copyright rule, persona role-play rule
2. `checklist.md`
3. `01-concept-brief.md` (MVP scope) and `project-plan.md` (Decisions)
4. `research/journey.md` → `research/user-stories.md`
5. `research/persona.md` as needed

## Decided in this session (don't reopen)
- **Persona candidates (2026-11-21):** log today + yesterday; mood = how the pages felt; paper card + home-screen shortcut (no reminders); theme and idea = two free-text fields; heavy day → room first, then "what's clearer now?" (never cheer up; help resources only if I turn them on); weekly patterns in the day-7 check-in, "new pattern" card parked; bilingual notes + manual theme merge, English UI; irregular writing is normal; success = insight, not completion.
- **Journey candidates (2026-11-27):** an always-available "so far" recap (progress, moods, ideas) as a mode of the pattern view; one tap turns an idea into the next artist date; the pattern view leads with recurring ideas, moods and themes as context; "start again from week 1" exists but is secondary; "pause" gets renamed.
- **Role-play rules that became criteria:** wordless "heavy" option (R1); one line max in hard moments (R2); check-in leads with what surfaced (R3); no gap count anywhere (R4); "nothing to log today" is a calm, complete state (R5).

## Waiting for my decision
1. The 4 open questions in `research/user-stories.md` (export; cut-line order of the Should stories; data threshold; what a real ending feels like).
2. **Paper prototype:** PM recommends starting it now in the notebook margin (mood · 1–2 themes · one idea, ~30 s per session). It's the only way to test the ideas-first pattern view with real data. Not yet confirmed.
3. Optional second archetype: PM recommends **skip** (I have kids, so the time-starved parent mostly duplicates the primary persona).

## Next tasks (Phase 2)
1. Decide the items above; review the user stories.
2. **Persona walkthrough** on Mobbin (competitor onboarding + check-in flows, as the persona) → artifact.
3. **Fresh-eyes review:** 5 independent designer subagents with only brief + persona + journey + user stories → `research/synthesis.md`.
4. **Scope the MVP:** confirm the story list as the v1 feature list; park the rest.
5. Handoff to Phase 3 (Design) with `project-scope.md`.

## Environment notes
- Mobbin connector works (when connected). Web pages: fetch allowed hosts with `curl` (see the 2026-11-21 notes in git history); 750words.com blocks automated visits.

## First prompt for the new session
> Read HANDOFF.md, then CLAUDE.md, and tell me where we are. Then walk me through the open questions in the user stories one by one, and after that start the persona walkthrough on Mobbin.
