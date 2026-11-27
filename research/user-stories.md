# User stories: Artist's Sketchbook v1
**Phase 2: Discovery, step "Scope the MVP" · 2026-11-27 · draft v1 (for my review)**
**Built from:** `01-concept-brief.md` (MVP scope), `research/persona.md` v4, `research/journey.md` v2 and every decision in `project-plan.md` up to 2026-11-27.

## How to read this
- Format: **As a returning creative, I want … so that …**, then **acceptance criteria** (testable; these become the Phase 5 eval criteria) and the **source** (decision, journey step or role-play finding R1–R7).
- **Priority:** **Must** = v1 doesn't work without it · **Should** = in v1, first to cut if the build runs long, in this order: US-21 → US-15 → US-18.
- Copy rule for every story: our own words, never the book's text; hard moments get **one line, max** (R2).
- Wording: "pages" are always the handwritten ones. The app never stores or reads them.

## Cross-cutting criteria (apply to every story)
- **X1 Accessibility:** AA contrast; status never shown by color alone; touch targets ≥ 44 px; works with a screen reader; respects reduced motion; Cyrillic-ready fonts.
- **X2 No judgment:** no streaks, no gap counts, no percentages or targets, no red "missed" states, anywhere (R4, decision "irregular writing is normal").
- **X3 Privacy:** data stays in my saved data; nothing is sent elsewhere; no account.
- **X4 Language:** UI in English; my notes accept Bulgarian and English.
- **X5 Mobile-first:** everything works one-handed at phone width.

---

## E1. Starting the course
**US-01 Start the course** · Must
As a returning creative, I want to start by picking a start date so that week 1 begins when I'm ready, not on a fixed weekday.
- [ ] A start date can be today or a chosen date; week 1 begins on it.
- [ ] Onboarding is at most 2 screens and can be finished in under a minute.
- [ ] The first screen says, in one or two lines, that the pages stay on paper and the app only keeps my short notes.
- [ ] Nothing in onboarding mentions streaks, daily targets or "don't break the chain".
*Source: start-day decision; journey step 0 (break the "tracker = judge" model).*

**US-02 Add to home screen** · Must
As a returning creative, I want a home-screen shortcut so that the app opens in one tap from my phone.
- [ ] Onboarding shows how to add the app to the home screen (iOS and Android), skippable.
- [ ] From the home-screen icon, "Pages done" is reachable with one more tap.
*Source: decision "paper cue + shortcut".*

**US-03 The notebook card** · Must
As a returning creative, I want a small card to keep in my notebook so that the one thing I always have when I write reminds me of the app.
- [ ] A printable card (or a design to copy by hand) with a QR code or link to the app.
- [ ] Its wording talks about *when* I write, never "every day", and makes no promise I could break (R4).
- [ ] Offered during onboarding and again from settings.
*Source: decision "paper cue + shortcut"; journey step 5 (the dread starts at the card).*

## E2. Pages done and the 10-second capture
**US-04 Pages done in one tap** · Must
As a returning creative, I want to mark my pages done in one tap so that logging never gets in the way of the practice.
- [ ] From opening the app to "done" takes **under 5 seconds**.
- [ ] Wording is neutral ("Pages done"), never "this morning".
- [ ] Shorter pages count: a quiet option to mark them shorter, never the default ask.
- [ ] Tapping twice on the same day doesn't create two entries; it can be undone.
*Source: brief constraint #1; decisions "a shorter morning counts", "log late".*

**US-05 Log yesterday** · Must
As a returning creative, I want to log yesterday's pages so that remembering late doesn't count as missed.
- [ ] Logging for yesterday is one obvious control on the Today screen, not a hidden date picker.
- [ ] Days older than yesterday can't be backfilled; they go through the comeback (US-10).
*Source: decision "log late: today + yesterday"; journey step 2.*

**US-06 Optional capture** · Must
As a returning creative, I want to note how the pages felt, 1–2 themes and one idea, only when I want to, so that patterns build up without it feeling like homework.
- [ ] The capture appears **only after** "Pages done" and takes about **10 seconds**.
- [ ] **Skip** is as visible as Save; every field is optional; a capture with only a mood is valid.
- [ ] The mood question asks **how the pages felt**, not how I feel now.
- [ ] Theme (what the pages were about) and idea (one creative idea) are **two free-text fields**; no medium picker.
- [ ] Both fields suggest my own past entries, in either language.
- [ ] A capture can be edited or deleted later.
*Source: decisions on mood, capture fields, bilingual notes; journey step 1.*

**US-07 A heavy morning** · Must
As a returning creative, I want the app to make room when the pages were heavy so that I can leave it without being chased away.
- [ ] One of the mood choices means "heavy" **without needing a word for the feeling** (R1).
- [ ] Choosing it shows **one line** that the heavy part is done and an early dip is normal.
- [ ] Then an **optional** "what's clearer now?" field; skipping it is one tap and nothing follows.
- [ ] An idea saved here is marked as "after a heavy page" for the pattern view.
- [ ] The app does **not** cheer me up, ask why, or show patterns in this moment.
- [ ] Help resources appear **only if I've turned them on** in settings (US-21).
*Source: decision "what's clearer now?"; journey step 3; R1, R2.*

## E3. Coming back
**US-08 Nothing to log today** · Must
As a returning creative, I want opening the app on a day without pages to feel complete so that just opening it never makes me feel worse.
- [ ] With no pages today (and yesterday already logged or skipped), the Today screen is calm and finished-looking, not an empty to-do.
- [ ] No prompt asks me to write, explain or log anything.
- [ ] The pattern view and artist date are reachable but not pushed.
*Source: journey step 6; R5.*

**US-09 No gap shown, ever** · Must
As a returning creative, I want days without pages to stay blank so that a gap never looks like failure.
- [ ] No screen shows a count of missed days or a broken streak, however kindly worded (R4).
- [ ] Calendar or timeline views show days without pages as simply empty, with no color or icon meaning "missed".
*Source: X2; journey steps 2, 5; R4.*

**US-10 Come back after a few days** · Must
As a returning creative, I want the app to open on today after a gap so that I can just carry on.
- [ ] After 2+ days without a log, the app opens on today with **one** welcome-back line ("when you write" framing).
- [ ] It doesn't ask me to explain or fill in the gap; yesterday can still be logged (US-05).
*Source: decision "comeback is a core flow"; journey steps 5–6.*

**US-11 Come back after a missed week** · Must
As a returning creative, I want to choose how to continue after a week away so that I never have to start over unless I want to.
- [ ] After 7+ days without a log, I see two primary choices: **pick up where I left off** or **join the current week**. Neither is styled as the "right" one.
- [ ] **Start again from week 1** is available as a secondary option (e.g. a text link), never a primary button or default.
- [ ] One sentence of inspiration, our own words.
- [ ] The word "pause" isn't used in a way that reads as "wait until you're ready" (R7).
*Source: decisions on missed week (2026-11-15, 2026-11-27); journey step 8; R7.*

## E4. The pattern view
**US-12 Ideas first** · Must
As a returning creative, I want the pattern view to lead with my recurring ideas so that I see what keeps calling me, not just what I already know.
- [ ] The top of the pattern view shows ideas, with recurring ones grouped and counted plainly (e.g. "came up 3 times").
- [ ] Each idea shows its context: how the pages felt that day and the themes around it.
- [ ] Ideas written after a heavy page can be seen as such.
- [ ] Moods over time and recurring themes come after, as context.
*Source: decision "pattern view leads with ideas"; journey step 7a; R6.*

**US-13 Useful with little data** · Must
As a returning creative, I want the pattern view to make sense with only a few irregular notes so that week 5 isn't a disappointment.
- [ ] With fewer than ~5 captures it shows a "so far" list, not charts.
- [ ] Weeks 1–2: visible, with a calm empty state and no pushed insights.
- [ ] No wording ever suggests writing more or differently to get "better" patterns (Q4 writing for the tag).
*Source: decision "pattern view low-key in weeks 1–2"; journey step 7a.*

**US-14 Merge themes** · Must
As a returning creative, I want to merge themes that mean the same thing ("работа" + "work") so that writing in two languages doesn't split my patterns.
- [ ] I can merge two or more themes and pick the name that shows.
- [ ] A merge can be undone.
- [ ] Future suggestions use the merged theme.
*Source: decision "bilingual notes with manual merge".*

**US-15 "So far" recap, any time** · Should
As a returning creative, I want a recap of my progress, moods and ideas so far, open any time, so that insight counts whenever I stop.
- [ ] A "so far" mode of the pattern view, available from day 1.
- [ ] Progress is plain numbers only (weeks, page days, artist dates); no percentages or targets (X2).
- [ ] Moods are shown as context for ideas and as what helped; never interpreted or diagnosed.
*Source: decision "always-available recap" (2026-11-27); success = insight.*

**US-16 Accessible patterns** · Must
As a returning creative using a screen reader or without color, I want every pattern available as text so that nothing depends on seeing a chart.
- [ ] Every chart has a text equivalent; moods are never color-only.
*Source: brief accessibility criteria.*

## E5. Artist dates
**US-17 Plan an artist date** · Must
As a returning creative, I want to plan a small artist date so that it fits a week with work and kids.
- [ ] Plan is optional text and an optional day; no time slot required.
- [ ] Suggestions are small (about 30 minutes, possible at home) and span my media (drawing, writing, photo, crafts, singing, video). Our own content.
- [ ] Weeks 1–4: suggestions lean toward permission ("small counts").
*Source: brief; persona (permission, time, kids); journey step 2.*

**US-18 Idea → artist date** · Should
As a returning creative, I want to turn one of my ideas into my next artist date in one tap so that recurring ideas turn into something I do.
- [ ] Each idea in the pattern view has "Make it my next artist date".
- [ ] The plan opens prefilled with the idea's text, editable.
- [ ] The date stays linked to the idea.
*Source: decision 2026-11-27; journey step 7b.*

**US-19 Mark a date done + what came out of it** · Must
As a returning creative, I want to mark a date done and note what came out of it so that I see what my practice produces.
- [ ] Done is one tap; the note is optional, one sentence, text only.
- [ ] In the pattern view the note appears next to the idea it came from, if any (idea → date → what came out).
- [ ] A week with no date is shown neutrally, with no "missed" state.
*Source: decision "what came out of it?" note; US-18.*

## E6. The week and the course
**US-20 Day-7 check-in** · Must
As a returning creative, I want an invited check-in on my day 7 that shows me what surfaced so that I notice patterns without being graded.
- [ ] Invited on day 7 of my week; can be dismissed; the next week opens either way (weeks never lock).
- [ ] Pages and artist date are **prefilled** from my taps.
- [ ] It **leads with what surfaced** (recurring themes, ideas, links); counts come after, small and neutral (R3).
- [ ] A missing artist date: one neutral line + one small, at-home suggestion.
- [ ] One optional reflection line, our own wording.
- [ ] Takes **under 2 minutes**.
*Source: check-in decisions; decision "weekly patterns in the day-7 check-in"; journey step 4; R3.*

**US-21 Help resources, only if I choose** · Should
As a returning creative, I want to decide whether the app ever shows help resources so that it never acts like a mental-health tool unless I ask.
- [ ] Off by default; turned on in settings.
- [ ] When on, a quiet link appears on heavy days; never a pop-up.
*Source: decision 2026-11-21 (heavy-day "never" list).*

**US-22 Light 12-week path** · Must
As a returning creative, I want to see which week I'm in and its theme so that I feel the course frame without homework.
- [ ] Current week number and a short theme in our own words; all 12 weeks visible, none locked.
- [ ] No weekly task lists.
*Source: brief; weekly tasks parked.*

**US-23 Early support, weeks 1–4** · Must
As a returning creative, I want extra permission and calm in the first weeks so that I get past where I've stopped before.
- [ ] Weeks 1–4 show short permission framing in the places above (capture, check-in, artist date), tapering week by week.
- [ ] From week 5 it's gone unless a heavy day calls for the US-07 line.
*Source: decision "early support weeks 1–4, tapering".*

**US-24 Course complete** · Must
As a returning creative, I want a closing moment after week 12 that looks back at what surfaced so that the course has an ending.
- [ ] Shown once after week 12; reopenable.
- [ ] Leads with recurring ideas and what my dates produced, not stats (uses US-15).
- [ ] No confetti-style celebration unless I decide otherwise in Phase 4.
*Source: brief; journey step 10.*

## E7. My data
**US-25 Saved between visits** · Must
As a returning creative, I want my logs and notes to persist so that weeks of patterns are never lost.
- [ ] Data survives closing the app, reloading and coming back weeks later.
- [ ] One "Download my notes" control in settings saves a plain text/CSV file: dates, moods, themes, ideas, artist dates and their notes.
- [ ] Export only; no import in v1 (parked for v1.1).
*Source: brief; X3; decision 2026-11-27 (export only).*

---

## Not in v1 (see `ideas.md`)
"New pattern" card · Bulgarian UI · import from export file (v1.1) · linking patterns to my creative goal · reminders · AI handwriting scan · photos for date notes · weekly tasks · share card (v1.1) · testers' demo copy (Phase 7).

## Open questions
1. ~~**Export (US-25):**~~ ✅ decided 2026-11-27: keep (Must), export only; import parked for v1.1.
2. ~~**Priority cut line:**~~ ✅ decided 2026-11-27: if the build runs long, cut US-21 → US-15 → US-18 (US-18 last).
3. **US-13 threshold:** "~5 captures" before anything beyond a list is a guess; the paper prototype would set it.
4. **US-24:** what would feel like a real ending? (still open from the journey)
