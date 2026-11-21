# The Artist's Way App — Start-to-Finish Checklist

> **Reconcept 2026-11-15:** moved from Atomic Habits to *The Artist's Way* (the official Atoms app was too close). Old brief: `archive/01-concept-brief-atomic-habits.md`.

Based on [`workshop-video/process-tutorial.md`](workshop-video/process-tutorial.md), adapted to this project:
personal use + portfolio case study · a companion for the 12-week course · mobile-first web · delivered as a working link.

**Adaptations from the workshop**
- No existing codebase → we create a small design system (`DESIGN.md`) instead of reusing a repo's.
- "Walk the real app as the persona" → walk competitor flows on Mobbin first, then our own prototype.
- "Ship a PR" → publish a working link (Claude artifact with saved data). GitHub is optional, for the portfolio.

**Session rule:** one Claude Code session per phase, all in this folder. When context gets heavy (~70%), ask for a handoff file and start the next session from it.

---

## Phase 0 — Setup
- [x] Create project folder `My New Claude UX Project`
- [x] Create a product designer persona file (`product-designer-persona.md`)
- [x] Connect Mobbin (Customize → Connectors) and test it
- [x] Write the project plan (`project-plan.md`)
- [x] Turn the persona into a short `CLAUDE.md` so every session reads it automatically (keep it lean; add a pointer to `project-plan.md`)
- [ ] Check `/context` at the start of each session to see what's loaded

## Phase 1 — Concept (session: *Concept*)
- [x] ~~Atomic Habits concept~~: drafted, reviewed critically, dropped (too close to Atoms) → archived
- [x] Pick a new book: **The Artist's Way** (no official app; 12-week structure)
- [x] Draft the new concept brief v1 (`01-concept-brief.md`)
- [x] Review the brief and approve the MVP scope
- [x] Answer the open questions: **name**, **falling behind** (pause vs move on), **tasks** (typed vs count), **start day**
- [x] Be critical: reread the brief and challenge anything that feels generic or "average" (9 fixes accepted)

## Phase 2 — Discovery (session: *Discovery*)
- [x] **Desk research** (done 2026-11-15 via direct web search, not subagents): reviews, Reddit/forums, app store complaints about habit trackers (why people quit; streak-loss frustration) → `research/user-complaints.md` (still applies to a daily practice)
- [x] **First: test the key assumption** (result: not supported; the real need is seeing my own patterns) (why an app if the work is on paper?) against my own past attempts at the course: where did I stall, what did paper fail to do? → `research/my-past-attempts.md`
- [x] Re-center the concept based on the interview → brief v2 (patterns, days 1–14 support; tasks parked)
- [x] **Artist's Way-specific research** (done 2026-11-16): others stall too, mostly weeks 1–5, for the same permission/time/emotional reasons; a real segment wants patterns but today's methods are heavy or need typing; trackers are checkbox logs → `research/artists-way-practitioners.md` (own file: a different question from habit-tracker complaints). all 4 candidates accepted 2026-11-21 (logged in Decisions)
- [x] **Competitor analysis** (done 2026-11-21; 4 decision candidates pending): typing apps own the morning-pages category; new scan-and-AI journals are paper-first but read the pages, so our edge is "the app never reads the pages"; only printables track the course: *Morning Pages* app, *AM Pages*, 750 Words, the 2012 *Artist's Way Toolkit*, Notion/printable trackers, the paper workbook — core loop, paper vs typing, what's missing → `research/competitors.md`
- [ ] **Persona** focused only on doing the course (not demographics): goals, frustrations, daily context, past attempts → `research/persona.md`
  - [ ] Primary: me (real data from my own mornings and past attempts at the course)
  - [ ] Optional: one more archetype for the portfolio story
- [ ] **User journey with mental model:** for each step, note what happened, what was expected, what they think, what they feel → `research/journey.md`
- [ ] **Persona walkthrough:** have the agent role-play the persona through competitor onboarding + habit-creation flows on Mobbin, screenshot each step, analyze reactions → artifact
- [ ] **Fresh-eyes review:** spawn 5 independent designer subagents with only the brief + persona + journey → `research/synthesis.md` (where do all 5 agree? what are the outliers?)
- [ ] **Scope the MVP:** confirm the v1 feature list; park everything else in `ideas.md`
- [ ] **Handoff:** `HANDOFF.md` + `project-scope.md` + a first prompt for the Design session

## Phase 3 — UX flows (session: *Design*)
- [ ] Map the core flows: **start the course** · **pages tap + 10 s capture** · **pattern view** · **artist date (plan/done)** · **weekly check-in** · **early support, weeks 1–4** · **light 12-week path** → `design/flows.md`
- [ ] Pattern research with 3 parallel Mobbin researchers, one per moment:
  - [ ] onboarding / starting a program
  - [ ] one-tap daily check-in
  - [ ] mood / reflection tracking + pattern and insight views (accessible, not color-only)
  → artifact "Habit App Patterns"
- [ ] List every state per screen: before start, first day, missed a day, missed a week (pause/continue choice), check-in skipped, week complete, course complete

## Phase 4 — UI design (session: *Design*, continued)
- [ ] **Visual direction:** pick ONE reference app to borrow the style from (don't mix 10)
- [ ] Create `DESIGN.md`: colors, type, spacing, components, plus **do / don't rules** for each
- [ ] Design key screens on the canvas inside Claude Code
- [ ] **Versioning rule:** each round of feedback = a new row of versions, never overwrite
- [ ] Explore copy variations (pages-done message, comeback copy, weekly check-in prompts in our own words)
- [ ] Make the boards playable prototypes; click through on phone width
- [ ] **Fresh-eyes review:** 2 subagents per prototype direction → pick a direction
- [ ] For each section/screen, find 1 Mobbin reference and copy it closely
- [ ] **Handoff** for the Build session

## Phase 5 — Build (session: *Build*)
- [ ] Have the agent write the build prompt from the handoff (I review and trim it)
- [ ] Build mobile-first web app as a Claude artifact with **saved data** (my pages log and check-ins persist between visits)
- [ ] Use only `DESIGN.md` tokens/components — no one-off styles
- [ ] **Real data, no mock data** — test with my actual pages and artist dates
- [ ] Ask the agent: "I expect gaps — find what we missed" (states, edge cases, empty screens)
- [ ] Verify like a designer: click every state, check on a real phone, Inspect element to confirm tokens
- [ ] **Evaluation skill:** create an eval skill with clear criteria (book fidelity without copying its text, accessibility, pages check-in under 5s, weekly check-in under 2 min) that runs in a fresh subagent → score → fix → re-run until 9+/10

## Phase 6 — Ship
- [ ] Publish the working link
- [ ] Use it through the 12 weeks; log friction in `feedback.md`
- [ ] Optional: put the code on GitHub for the portfolio

## Phase 7 — Test & iterate (v1.1)
- [ ] Decide on the **"share your week" card** (v1.1 candidate in `ideas.md`): would I actually share after a few weeks of use?
- [ ] Make a **separate demo copy** for testers (they must not see or overwrite my data), then share it with 3–5 people for feedback; give them 1–2 tasks (start the course, log pages, do a weekly check-in)
- [ ] Synthesize feedback → prioritize fixes
- [ ] Re-run the eval skill after changes
- [ ] 12-week self-test: did I finish the course with it?

## Phase 8 — Portfolio case study
- [ ] Export each session's chat transcript → have an agent analyze how I made decisions (my *real* process)
- [ ] Collect artifacts: brief, persona, journey, synthesis, pattern boards, design versions, final link
- [ ] Write the case study: problem → insight → key decisions (with rationale) → result → what I learned
- [ ] Publish the case study page and link the live app
