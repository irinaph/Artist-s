# Fresh-eyes review: synthesis
**Phase 2: Discovery · 2026-11-27**
**Inputs given to each reviewer (only these):** `01-concept-brief.md`, `research/persona.md` v4, `research/journey.md` v2, `research/user-stories.md` v1.1. They did **not** see `project-plan.md` (Decisions), the persona walkthrough, `ideas.md` or the paper prototype, so they couldn't lean on our reasoning.
**Raw reviews:** `research/fresh-eyes-reviews/reviewer-1.md` … `reviewer-5.md`

## Method
Five independent subagents got the same task and the same 8 headings, but each had a different professional background. When reviewers with different lenses agree, that's a stronger signal than five copies of one lens agreeing.

| # | Lens | Verdict in one line |
|---|---|---|
| R1 | Senior product designer (generalist) | Right product; the 12-week spine fits her less well than the docs assume |
| R2 | Accessibility & inclusive design | Right product, wrong data model: the stories assume a daily writer |
| R3 | Behaviour change & wellbeing | Right product, wrong unit of record: everything hangs off a "Pages done" she rarely produces |
| R4 | Content design / UX writing | Mostly yes; the data will be sparse and tilted toward heavy days |
| R5 | Design lead (build cost, scope) | Right product, still shaped like a daily tracker; biggest risk is data |

**All 5 agree on the main point.** The *product* is right for the persona. The *data model* still assumes someone who writes every morning, while the persona writes when she needs to unload. Nearly every finding below follows from that gap.

---

## Where all 5 (or 4 of 5) agree

| # | Finding | Who | Already covered? |
|---|---|---|---|
| A1 | **"Recurring ideas" has no mechanism.** Ideas are free text in two languages; merge exists only for themes (US-14). Without AI, "film the street at dusk" and "видео на залез" never match, so US-12 can't pass its own criteria. | 5/5 | **No. New.** This is the biggest gap. |
| A2 | **The time model is undefined.** "Pick up where I left off" (US-11) detaches course week from the calendar. Then what sets day 7 (US-20), the current week (US-22), weeks 1–4 (US-23), "after week 12" (US-24)? Plus: the day boundary for a 00:30 log; what counts as "a log"; a check-in not opened on day 7. | 5/5 | **No.** Flagged as a Phase 3 state list, but never as a model. |
| A3 | **The comeback flows will fire on her normal rhythm.** US-10 at 2+ days and US-11 at 7+ days are ordinary gaps for an irregular writer. "Welcome back" itself tells her the app counted her absence, so it's a soft gap count. | 5/5 | Partly. The tone is decided, but the triggers were set for a daily writer. |
| A4 | **Page-day counts are gap counts by subtraction.** "3 page days" in a 7-day check-in (US-20) or "9 page days" in week 6 (US-15) reads as 4 or 33 missed. X2 bans this in spirit; journey step 4 even has her react to it. | 5/5 | **No.** X2 and US-15/US-20 contradict each other. |
| A5 | **A mood history becomes a report card of her heavy days.** She writes to unload, so most captures will be heavy. "Moods over time" (brief, US-12, US-15) will chart her low points. | 5/5 | Partly. The journey decision made moods "context for ideas", but the brief and US-15 still list a mood series. |
| A6 | **Storage durability.** No account and export-only: browser storage can be cleared after a week unused (her missed-week case); the home-screen app and Safari keep separate storage. | 5/5 | **Mostly yes, in a way they couldn't see.** Our platform is a Claude artifact with saved data, not browser storage (Decisions, "Platform"). What's still open: does the private artifact open on the phone in one tap, logged in, from the home screen and the QR card? → Phase 5 spike. |
| A7 | **Ideas can only be logged after "Pages done".** The product's hook depends on her least frequent behaviour. Ideas from a commute or an artist date are lost. Bias: if ideas only come after pages, "most ideas came on heavy days" (journey 7b) is an artefact of *when* she's allowed to log. | 4/5 (R1, R2, R3, R5) | **No. New.** |
| A8 | **US-24 (course complete): build it late.** She has never passed day 10; there's no evidence for weeks 6–12. Keep the content decision; build it around week 8 of real use, with real data. | 5/5 | Content decided; build timing not. |
| A9 | **The wordless "heavy" option still needs a name.** US-07 says "no word for the feeling", but also "every option is icon + word". It works only if the word names the *weight*, not the emotion. A screen reader also needs a label for it, so that label is the real copy decision. | 5/5 | Partly (C3). The clarification is missing. |
| A10 | **"An early dip is normal" is false after week 4.** US-23 keeps the US-07 line from week 5 on; in week 9 "early" is wrong. | 4/5 | **No.** Simple copy fix. |
| A11 | **The cut order breaks a Must.** US-13's fallback with fewer than 5 captures *is* the "so far" list (US-15). Cutting US-15 first breaks US-13. Two "so far" things share one name. | 4/5 | **No.** Fix by moving the list into US-13. |
| A12 | **A Settings story is missing.** US-03, US-21 and US-25 point to it; nothing defines it (start date, card, resources, export, **delete all my data**). | 4/5 | **No.** |
| A13 | **Backfill from the dated notebook is blocked.** US-05 stops at yesterday, but real entries exist on paper. Blocking loses data and implies "those days are gone". | 4/5 | **Conflicts with a decision** (log late: today + yesterday, 2026-11-21). See S10. |
| A14 | **Privacy on a shared family phone.** Heavy-day notes and themes like "my sister" sit in an unlocked app; she has kids. | 4/5 | **No.** |
| A15 | **The brief is stale in 4 places:** "pause the path or continue" (replaced by US-11); "Morning: write pages" (no fixed time); "moods over time" first in the feature table (replaced by ideas first); the **2-week success criterion** (a new pattern by day 14) contradicts US-13 (low-key weeks 1–2, threshold 5). | 4/5 | **No.** |
| A16 | **The designer-as-user risk has no real mitigation.** Persona Q5/Q6 name it; the only mitigation is a demo copy in Phase 7. R1 goes further: role-play findings R1–R7 became Must criteria, which can read as self-confirming in the case study. | 4/5 | Partly (the evidence tags in the journey). |
| A17 | **A help resource as a minimal static line in Settings**, even with US-21 off and even if US-21 is cut. | 4/5 | Compatible with the "only if I choose" decision (Settings is a place she chooses to go). |
| A18 | **A Bulgarian note in an English UI needs `lang="bg"`**, or screen readers read Cyrillic with English rules. X4 covers input only. | 3/5 (+R5 on combobox semantics) | **No.** Add to X1. |

## The outliers (one or two reviewers, worth keeping)
- **R4: autocomplete inflates "recurring".** One tap on a suggested past entry is the easiest move in a 10 s capture, so counts rise because the suggestion was there, not because the idea came back. This is the writing-for-the-tag risk (persona Q4) built into the interaction. *Sharp. It shapes A1's solution:* suggest past **themes**, but link **ideas** explicitly.
- **R4: "what's clearer now?" isn't a creative idea.** After anger it's often a life insight ("talk to my sister"). Saving it as an idea puts something private next to "Make it my next artist date" (US-18). → store it as its own note type, with a one-tap "make it an idea".
- **R3: show the base rate, never a cause.** "6 of your 9 notes were after heavy pages", never "your ideas come from pain". R1 and R5 add: never frame distress as productive.
- **R4: a priority rule for what shows on open.** Check-in, missed-week choice and the post-course idea can all be due at once and collide with the 5 s target.
- **R5: 20 of 25 stories are Must.** Build a thin slice for week 1 and add the later-week features while using it (US-11 by week 2, US-24 by week 8).
- **R5: the QR card opens Safari, a second, empty copy** of a home-screen web app. *Matters for us too:* the card must open the same artifact, logged in. Goes into the Phase 5 spike (A6).
- **R1: tag every Must criterion with its evidence level** (research / my past attempts / role-play) and name which role-play findings the paper prototype must confirm.
- **R2, R4: "Pages done" undo must not hang on a disappearing toast** (WCAG 2.2.1); announce "done" in a live region (4.1.3).
- **R3, R4: dark mode is v1, not polish.** She writes in the kitchen before everyone wakes.
- **R2, R3, R5: cut the "shorter pages" toggle.** Nothing reads it, and it labels a lesser day. *Conflicts with a decision* (2026-11-21). See S9.
- **R2, R4, R5: simplify US-23's tapering** to on/off for weeks 1–4; tapering across three surfaces is about 12 copy variants.
- **R1, R3: demote US-14 (theme merge) to Should** if idea linking needs the room.
- **R3, R4: copyright.** The brief lists the book's 12 week-theme names; US-22 says "our own words". Decide which ships.

## What we missed (new to us)
1. **Idea recurrence needs a mechanism** (A1), and the obvious one, autocomplete, would fake it (R4).
2. **Ideas need their own entry point** (A7). Our model is pages-first; her value is ideas-first. We moved the *pattern view* to ideas first but left the *capture* pages-first.
3. **Our "no gap counts" rule has back doors**: page-day totals (A4), comeback triggers (A3), the mood series (A5).
4. **The time model** (A2): "pick up where I left off" was decided as a choice, not as a rule the rest of the app follows.
5. **The heavy-day note is a different kind of data** (R4).
6. **Delete all my data, Settings, a shared phone** (A12, A14).

## Where the reviewers were wrong or out of date
- **Storage (A6):** they assumed browser storage. Our Decisions say "Claude artifact with saved data". The risk shrinks to access: login, home screen, QR card.
- **"Shorter pages" has no purpose (S9):** they didn't see the 2026-11-21 reasoning (people who finished shrank the pages; the book's three pages stay the norm).
- **Backfill (A13):** they didn't see why we stopped at yesterday (so logging never becomes catch-up homework).

---

## Candidates for your decision
*PM recommendation first, then the trade-off. Nothing changes in the stories until you decide.*

**S1. Ideas are linked, not matched** (A1, R4) · *Recommend: accept, Must*
When she saves an idea, the app offers "same as an earlier idea?" with her recent ideas. One tap links them, and the count comes from the links. Past *themes* are still suggested as text; past *ideas* are not autocompleted. A merge for ideas in the pattern view (extending US-14) is the fallback.
*Trade-off:* one optional extra tap in the capture, and the hardest new widget. Without it, the headline of the pattern view is a list of one-offs.

**S2. "Add an idea" any time, without pages** (A7) · *Recommend: accept, Must*
A quiet second entry on Today. Each idea records where it came from (after pages / after a date / on its own). "Pages done" stays the main button and the 5 s target stays.
*Trade-off:* Today gets a second action. It also removes the heavy-day bias from the ideas data.

**S3. Write a one-page time and state model before the Phase 3 flows** (A2, R4) · *Recommend: accept, first Phase 3 task*
It covers: course week vs calendar, what "pick up" shifts (start date + offset), the day boundary (e.g. a new day starts at 4 a.m.), what counts as activity (any tap), a check-in not opened on day 7 (it stays open until the next week's, never stacks), and a priority rule for what shows on open (one thing at a time).
*Trade-off:* none really; it's the missing spine of E3 and E6.

**S4. Comebacks fit an irregular writer** (A3) · *Recommend: accept*
Drop the US-10 welcome-back line; the calm Today screen (US-08) *is* the comeback. Keep US-11's two equal cards (C4), but show them only after **14 days** with no activity of any kind, once per gap, as a card on Today she can dismiss, not a blocking screen. The C1 welcome line in onboarding stays.
*Trade-off:* a week away gets no acknowledgment. For you, a week away is normal, so that's the point.

**S5. Count only what I made** (A4) · *Recommend: accept*
No page-day totals in the check-in (US-20) or the recap (US-15). Counts are per idea ("came up 3 times"), artist dates done and notes written. The week number stays.
*Trade-off:* you lose a page tally. X2 already says no tallies in spirit.

**S6. Mood as context only, no mood timeline in v1** (A5, R3) · *Recommend: accept*
Mood shows next to each idea and in the check-in, never as a series over time. Any heavy-day link is a base rate ("6 of 9"), never a cause, never a headline. This finishes the journey decision "moods are context for ideas"; the brief's feature table gets updated.
*Trade-off:* "moods over time" leaves the brief. It may come back later, opt-in, once real data shows it's useful.

**S7. A heavy-day note is its own type** (R4) · *Recommend: accept*
The "what's clearer now?" answer is saved as a note, not an idea. One tap "make it an idea" promotes it. Only ideas appear in US-12 and US-18.
*Trade-off:* a second data type, but small.

**S8. Fix the copy and the stale brief** (A9, A10, A15, copyright) · *Recommend: accept all*
- US-07: the heavy option's word names the **weight** ("heavy"), not an emotion; it has a plain spoken label.
- After week 4, the heavy-day line drops "early".
- Brief: replace "pause or continue", "Morning:", the mood-first feature row, and restate the 2-week criterion to fit US-13 (e.g. "by week 4, at least one idea I'd forgotten, with its context").
- **Copyright:** remove the book's 12 week-theme names from the brief; US-22 uses our own short themes, written in Phase 4.

**S9. Scope and sequencing** (A8, A11, R5) · *Recommend: accept*
- Move the "so far" **list** into US-13; US-15 becomes only the recap mode, so the cut order (US-21 → US-15 → US-18) no longer breaks a Must.
- US-24 stays Must, but is built around week 8 of real use. Phase 5 builds a week-1 slice first.
- US-23: weeks 1–4 on/off, no week-by-week tapering in v1.
- **Keep the "shorter pages" option** (decided 2026-11-21); just make sure nothing ever shows it as lesser. *Outlier view:* cut it, because nothing reads it.

**S10. Backfill from the notebook** (A13) · *Recommend: keep the decision for now and test it*
Keep today + yesterday. Add one question to the paper prototype: "did I want to copy an older margin note in?" If yes, add an unprompted "add an earlier note" for captures only.
*Trade-off:* real entries may be lost for 1–2 more weeks, against a decision made to stop catch-up homework.

**S11. New stories: Settings, privacy, safety line** (A12, A14, A17) · *Recommend: accept the first, park the lock*
- **US-26 Settings** (Must): start date, notebook card, help-resources toggle, one static help line always there, "Download my notes", **delete all my data**.
- **App lock:** park in `ideas.md`. Cheap mitigation in v1: no note text on Today, so the first screen is safe for anyone to see.

**S12. Accessibility and evidence additions** (A18, R1, R2–R4) · *Recommend: accept*
- X1 adds: `lang="bg"` on Cyrillic notes; "done" announced in a live region; undo stays on Today (not a toast); dark mode in v1; suggestion lists as proper comboboxes.
- Each Must criterion gets an evidence tag (research / past attempts / role-play). The paper prototype names which role-play findings it must confirm.
- The **demo copy** moves from Phase 7 to Phase 5, so testing never touches my data (A16).

**Paper prototype, proposed additions** (S1, S2, S10; your prototype, so your call):
- On how many days did I write at all? (sets S4's threshold)
- Did ideas come **away from the pages**? Note them on a separate line. (tests S2)
- Did an idea come back **in different words**? Would I have linked them? (tests S1)
- Did I want to copy an older margin note in? (tests S10)
