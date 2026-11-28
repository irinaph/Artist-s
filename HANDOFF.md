# Handoff: Phase 2 (Discovery) done → Phase 3 (UX flows)
*Written 2026-11-28 at the end of the fresh-eyes review session. Replaces the 2026-11-27 handoff.*

## Where we are
- **Phases 0–1** done. **Phase 2 (Discovery)** is done, except for reading the paper prototype after week 1, which doesn't block Phase 3.
- **Scope:** `project-scope.md` v1 (provisional) is the map; `research/user-stories.md` v1.2 (28 stories) is the source of truth.
- **Git:** all work is on `claude/brave-gauss-ueqt2x` (pushed; it includes `adoring-allen`'s last commit). `main` is behind; merge when I decide.

## Done in this session (don't reopen)
- **Second archetype:** skipped. **Journey v2:** signed off.
- **Fresh-eyes review** → `research/synthesis.md` + raw reviews in `research/fresh-eyes-reviews/`. 5 independent reviewers; the main finding (5/5): the data model still assumed a daily writer.
- **S1–S12 + S1b all accepted** (see Decisions, 2026-11-27). Key changes:
  - ideas are linked by me (US-28), with **opt-in AI-suggested links I confirm**
  - "Add an idea" any day (US-27)
  - no welcome-back line; the missed-week card appears after 14 days with no activity
  - count only what I made, never page days
  - mood only as context, no timeline
  - "what's clearer now?" is saved as a note
  - new US-26 Settings with "delete all data"
  - the book's week-theme names removed
  - evidence tags on every story
  - demo copy moved to Phase 5
- **Positioning:** "the market leader's AI reads your pages. Ours **connects** your own ideas." "AI shapes my ideas" is parked in `ideas.md` (v1.1).
- **Paper prototype:** +4 questions (days written, ideas away from the pages, the same idea in new words, wanting older notes).
- Parked in `ideas.md`: app lock, mood timeline (opt-in).

## Read these first
1. `CLAUDE.md`, then `checklist.md` (Phase 3)
2. `project-scope.md`
3. `research/user-stories.md` v1.2
4. `project-plan.md` → Decisions (latest entries)
5. As needed: `research/journey.md`, `research/persona-walkthrough.md`, `research/synthesis.md`

## Next tasks (Phase 3)
1. **The time and state model** (S3), at the top of `design/flows.md`: course week vs calendar and what "pick up" shifts; the day boundary; what counts as activity; a check-in not opened on day 7; one thing at a time on open.
2. **Map the core flows**, including the new ones: add an idea, link ideas (manual + AI suggestions), settings.
3. **List every state per screen.**
4. **Mobbin pattern research** (3 parallel researchers: onboarding, check-in + capture, pattern/insight views).
5. **Around 2026-12-04:** read the paper prototype's week 1 → update US-13 (threshold), US-11 (14 days), US-27/28, US-05, and `project-scope.md`.

## Waiting for my decision
- Nothing open. Merging `claude/brave-gauss-ueqt2x` into `main` is up to me.

## Environment notes
- The Mobbin connector works when connected. Walkthrough screen previews live only in the artifact https://claude.ai/artifact/LcjnxUEJY4QxoNzEN5xth7 (private).
- 750words.com blocks automated visits.
- The Phase 5 spike also has to check that an artifact page can call Claude (needed for S1b).

## First prompt for the new session
> Read HANDOFF.md, then CLAUDE.md, and tell me where we are. Then start Phase 3 with the time and state model at the top of design/flows.md.
