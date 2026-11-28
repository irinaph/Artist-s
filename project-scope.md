# Project scope: Artist's Sketchbook v1
**End of Phase 2 (Discovery) → input for Phase 3 (UX flows) · 2026-11-28 · v1 (provisional: adjust after week 1 of the paper prototype)**

## In one line
A personal, mobile-first web companion for the 12-week *Artist's Way* course. The pages stay on paper. One tap logs them, an optional 10-second note captures mood, themes and an idea, and the app shows me my **recurring ideas** with their context. AI only connects my own ideas, and only if I turn it on.

**User:** me only (`research/persona.md` v4, "The Returning Creative"). I write irregularly, when I need to unload. Both past attempts ended in weeks 1–2.
**Platform:** a Claude artifact with saved data, mobile-first web, opened from a home-screen icon and a QR card in my notebook.
**Positioning:** the market leader's AI reads your pages. Ours connects your own ideas.

## The v1 feature list
The source of truth is `research/user-stories.md` v1.2 (28 stories with acceptance criteria). This is the map.

| Epic | Must | Should |
|---|---|---|
| **E1 Starting the course** | US-01 start date (≤ 2 screens, welcome-back line) · US-02 home-screen shortcut · US-03 notebook card | |
| **E2 Pages + capture** | US-04 "Pages done" in one tap (< 5 s) · US-05 log yesterday · US-06 optional 10 s capture · US-07 a heavy morning · US-27 add an idea any time | |
| **E3 Coming back** | US-08 nothing to log today · US-09 no gap shown, ever · US-10 back after a few days (no line) · US-11 after 14 days: two equal cards | |
| **E4 Pattern view** | US-12 ideas first · US-13 useful with little data ("so far" list) · US-14 merge themes · US-16 accessible patterns · US-28 link the same idea (+ opt-in AI suggestions) | US-15 recap mode |
| **E5 Artist dates** | US-17 plan · US-19 done + "what came out of it?" | US-18 idea → artist date |
| **E6 Week and course** | US-20 day-7 check-in · US-22 light 12-week path · US-23 early support weeks 1–4 · US-24 course complete | US-21 help resources |
| **E7 My data** | US-25 saved + "Download my notes" · US-26 Settings (incl. delete all data) | |

**Cross-cutting rules for every screen:** X1 accessibility (AA, never color-only, 44 px, screen reader, reduced motion, `lang="bg"`, live regions, no timed toasts, dark mode) · X2 no judgment (no streaks, gap counts, page-day totals, targets, red states, or mood timeline) · X3 privacy (no account; only idea text goes to AI, opt-in) · X4 English UI, notes in Bulgarian or English · X5 one-handed at phone width.

**Cut order if the build runs long:** US-21 → US-15 → US-18.
**Build order:** week-1 slice first (E1, E2, US-08, US-09, US-25, US-26, US-27) → US-11 by my week 2 → the rest during use → US-24 by week 8.

## Not in v1
Everything else is parked in `ideas.md` with its user problem and when to revisit it.
- **v1.1:** share card · import from export · letter to future me · AI shapes my ideas.
- **Later:** app lock · mood timeline · "new pattern" card · Bulgarian UI · patterns linked to my goal · AI handwriting scan · photos for date notes · weekly tasks · opening to core users · community · reminders.

## Constraints
- **Copyright:** no text from the book: no task lists, check-in questions, quotes or week-theme names. Week themes and all suggestions are our own words (Phase 4).
- **Trademark:** "The Artist's Way" is never in the app's name. Check "Artist's Sketchbook" before launch.
- **"Pages done" in under 5 s** is the #1 build constraint. The capture and "Add an idea" take about 10 s. The weekly check-in takes under 2 min.
- **Not a mental-health tool:** calm copy, one line on hard moments. No cheering up, no interpretation, no therapy-like features.
- **The AI limit:** it only proposes pairs of my ideas, and I confirm each one. It never summarises, interprets, or touches pages, moods, themes or notes.
- **The avoid list** (for `DESIGN.md`): account wall · setup theatre · praise after input · small Skip · streaks anywhere · lost/missed/relapsed/repair/freeze · color-only or red valence · "most missed" · AI interpretation, affirmations or plans · completion rates and scores · proof of practice.

## Success criteria
- **Main:** 6 weeks with real insight. Stretch goals: day 14, week 4, all 12 weeks.
- **By week 4**, the pattern view shows me at least one idea I'd forgotten, with its context.
- **Speed:** "Pages done" < 5 s, capture about 10 s, check-in < 2 min.
- **Traceability:** every decision traces to the book, research or my own use (`project-plan.md` → Decisions).

## Still open (does not block Phase 3)
| Item | Decided by | Affects |
|---|---|---|
| Pattern threshold (5 captures, provisional) | Paper prototype, week 1 (around 2026-12-04) | US-13 |
| Comeback threshold (14 days) | Prototype: days written | US-11 |
| Do ideas come away from the pages? Is linking needed? | Prototype questions 8–9 | US-27, US-28 |
| Backfill older than yesterday | Prototype question 10 | US-05 |
| Artifact opens in one tap, logged in, from icon + QR; the page can call Claude | Phase 5 spike (it shapes US-02, US-03, US-28, so check early) | US-02, US-03, US-25, US-28 |

## Phase 3 starts with
1. **The time and state model** (S3), at the top of `design/flows.md`:
   - course week vs calendar, and what "pick up where I left off" shifts
   - the day boundary (e.g. 4 a.m.)
   - what counts as activity
   - a check-in not opened on day 7
   - one thing at a time on open
2. **The core flows:** start · pages + capture + add an idea · pattern view + linking · artist date · day-7 check-in · comeback · early support · 12-week path · course complete · settings.
3. **Every state per screen**, then the Mobbin pattern research (`checklist.md`, Phase 3).
