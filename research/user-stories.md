# User stories: Artist's Sketchbook v1
**Phase 2: Discovery, step "Scope the MVP" · 2026-11-27 · v1.2 (fresh-eyes candidates S1–S12 folded in; see `research/synthesis.md`)**
**Built from:** `01-concept-brief.md` (MVP scope), `research/persona.md` v4, `research/journey.md` v2 and every decision in `project-plan.md` up to 2026-11-27.

## How to read this
- Format: **As a returning creative, I want … so that …**, then **acceptance criteria** (testable; these become the Phase 5 eval criteria) and the **source** (decision, journey step or role-play finding R1–R7).
- **Priority:** **Must** = v1 doesn't work without it · **Should** = in v1, first to cut if the build runs long, in this order: US-21 → US-15 → US-18.
- **Evidence** (S12): each story ends with an *Evidence* line: **research** (desk research, practitioners, competitors), **past** (my past attempts), **decision** (a design call with no direct evidence), **role-play** (R1–R7, an agent playing me; treat as an assumption until the paper prototype or real use confirms it).
- **Build order** (S9): Phase 5 builds a **week-1 slice** first (E1, E2, US-08, US-09, US-25, US-26, US-27); the rest is added while I use it: US-11 by week 2, US-24 by week 8.
- **Time model** (S3): E3 and E6 depend on the one-page time and state model, the first Phase 3 task (`design/flows.md`).
- Copy rule for every story: our own words, never the book's text; hard moments get **one line, max** (R2).
- Wording: "pages" are always the handwritten ones. The app never stores or reads them.

## Cross-cutting criteria (apply to every story)
- **X1 Accessibility:** AA contrast; status never shown by color alone; touch targets ≥ 44 px; works with a screen reader; respects reduced motion; Cyrillic-ready fonts; Cyrillic notes shown with `lang="bg"`; confirmations (e.g. "Pages done") announced in a live region; undo stays on screen, never on a timed toast; dark mode in v1; suggestion lists are proper comboboxes.
- **X2 No judgment:** no streaks, no gap counts, no percentages or targets, no red "missed" states, anywhere (R4, decision "irregular writing is normal"). **Count only what I made** (ideas, artist dates, notes), never page days: a page-day total is a gap count by subtraction (S5). No mood timeline (S6).
- **X3 Privacy:** data stays in my saved data; no account. The only thing ever sent to AI is my idea text, and only if I've turned on idea links (S1b); the pages, moods, themes and notes are never sent.
- **X4 Language:** UI in English; my notes accept Bulgarian and English.
- **X5 Mobile-first:** everything works one-handed at phone width.

---

## E1. Starting the course
**US-01 Start the course** · Must
As a returning creative, I want to start by picking a start date so that week 1 begins when I'm ready, not on a fixed weekday.
- [ ] A start date can be today or a chosen date; week 1 begins on it.
- [ ] Onboarding is at most 2 screens and can be finished in under a minute.
- [ ] The first screen says, in one or two lines, that the pages stay on paper and the app only keeps my short notes.
- [ ] One line on the first screen welcomes a return (starting again is normal; the course begins from the date I pick). No question, no branching (C1).
- [ ] Nothing in onboarding mentions streaks, daily targets or "don't break the chain".
*Source: start-day decision; journey step 0 (break the "tracker = judge" model); walkthrough C1.* · *Evidence: past, decision, role-play (C1).*

**US-02 Add to home screen** · Must
As a returning creative, I want a home-screen shortcut so that the app opens in one tap from my phone.
- [ ] Onboarding shows how to add the app to the home screen (iOS and Android), skippable.
- [ ] From the home-screen icon, "Pages done" is reachable with one more tap.
*Source: decision "paper cue + shortcut".* · *Evidence: research (routine cues), decision.*

**US-03 The notebook card** · Must
As a returning creative, I want a small card to keep in my notebook so that the one thing I always have when I write reminds me of the app.
- [ ] A printable card (or a design to copy by hand) with a QR code or link to the app.
- [ ] Its wording talks about *when* I write, never "every day", and makes no promise I could break (R4).
- [ ] The QR/link opens the same app and data as the home-screen icon (Phase 5 spike).
- [ ] Offered during onboarding and again from settings (US-26).
*Source: decision "paper cue + shortcut"; journey step 5 (the dread starts at the card).* · *Evidence: past, role-play (R4).*

## E2. Pages done and the 10-second capture
**US-04 Pages done in one tap** · Must
As a returning creative, I want to mark my pages done in one tap so that logging never gets in the way of the practice.
- [ ] From opening the app to "done" takes **under 5 seconds**.
- [ ] Wording is neutral ("Pages done"), never "this morning".
- [ ] Shorter pages count: a quiet option to mark them shorter, never the default ask, and never shown anywhere as lesser.
- [ ] Tapping twice on the same day doesn't create two entries; it can be undone, with undo staying on Today (not a timed toast).
- [ ] "Done" is announced to screen readers.
*Source: brief constraint #1; decisions "a shorter morning counts", "log late".* · *Evidence: research (practitioners shrank the pages), past.*

**US-05 Log yesterday** · Must
As a returning creative, I want to log yesterday's pages so that remembering late doesn't count as missed.
- [ ] Logging for yesterday is one obvious control on the Today screen, not a hidden date picker.
- [ ] Days older than yesterday can't be backfilled; they go through the comeback (US-10). *(Kept 2026-11-27; the paper prototype tests whether I want to copy older notes in, S10.)*
- [ ] A new day starts at the time set in the time model (e.g. 4 a.m.), so a 00:30 log belongs to the night's day.
*Source: decision "log late: today + yesterday"; journey step 2.* · *Evidence: decision.*

**US-06 Optional capture** · Must
As a returning creative, I want to note how the pages felt, 1–2 themes and one idea, only when I want to, so that patterns build up without it feeling like homework.
- [ ] The capture appears **only after** "Pages done" and takes about **10 seconds**.
- [ ] **Skip** is as visible as Save; every field is optional; a capture with only a mood is valid.
- [ ] The mood question asks **how the pages felt**, not how I feel now.
- [ ] Theme (what the pages were about) and idea (one creative idea) are **two free-text fields**; no medium picker.
- [ ] The theme field suggests my own past themes, in either language. The idea field does **not** autocomplete past ideas (it would inflate "recurring", S1); linking happens later (US-28).
- [ ] An idea saved here is marked as coming "after pages".
- [ ] The capture has no extra linking step; it stays about 10 seconds.
- [ ] A capture can be edited or deleted later.
*Source: decisions on mood, capture fields, bilingual notes; journey step 1; fresh-eyes S1.* · *Evidence: past, decision, research (fresh-eyes 5/5 on idea grouping).*

**US-27 Add an idea any time** · Must
As a returning creative, I want to save an idea on any day, without pages, so that ideas from a commute or an artist date aren't lost.
- [ ] A quiet "Add an idea" action on Today, secondary to "Pages done".
- [ ] One text field; saving takes about 10 seconds; no mood or theme asked.
- [ ] Each idea records where it came from: after pages, after an artist date, or on its own; the pattern view can show this.
- [ ] It never counts as, or asks about, pages.
*Source: fresh-eyes S2 (4/5 reviewers); persona (writes when she needs to; goal 2 creative direction).* · *Evidence: research (fresh-eyes), past.*

**US-07 A heavy morning** · Must
As a returning creative, I want the app to make room when the pages were heavy so that I can leave it without being chased away.
- [ ] One of the mood choices means "heavy" **without needing a word for the feeling** (R1): its word names the **weight** ("heavy"), not an emotion, and it has a plain spoken label for screen readers.
- [ ] Every mood option is an icon + a word; none relies on color (C3, X1).
- [ ] Choosing it shows **one line** that the heavy part is done; in weeks 1–4 it adds that an early dip is normal; from week 5 it drops "early".
- [ ] Then an **optional** "what's clearer now?" field; skipping it is one tap and nothing follows.
- [ ] The answer is saved as a **note**, not an idea (S7); one tap "make it an idea" turns it into an idea marked "after a heavy page". Notes never appear in the ideas list or next to "Make it my next artist date".
- [ ] The app does **not** cheer me up, ask why, or show patterns in this moment.
- [ ] Help resources appear **only if I've turned them on** in settings (US-21).
*Source: decision "what's clearer now?"; journey step 3; R1, R2; fresh-eyes S7, S8.* · *Evidence: past (attempt 2 ended on anger), research (early dip), role-play (R1, R2).*

## E3. Coming back
**US-08 Nothing to log today** · Must
As a returning creative, I want opening the app on a day without pages to feel complete so that just opening it never makes me feel worse.
- [ ] With no pages today (and yesterday already logged or skipped), the Today screen is calm and finished-looking, not an empty to-do.
- [ ] No prompt asks me to write, explain or log anything.
- [ ] The pattern view and artist date are reachable but not pushed.
- [ ] Today shows no note or idea text, so the first screen is safe for anyone holding the phone (S11).
- [ ] When several things are due (check-in, comeback card, post-course idea), Today shows one at a time, by the time model's priority rule (S3).
*Source: journey step 6; R5; fresh-eyes S3, S11.* · *Evidence: role-play (R5), decision.*

**US-09 No gap shown, ever** · Must
As a returning creative, I want days without pages to stay blank so that a gap never looks like failure.
- [ ] No screen shows a count of missed days or a broken streak, however kindly worded (R4).
- [ ] Calendar or timeline views show days without pages as simply empty, with no color or icon meaning "missed".
- [ ] No page-day totals anywhere (S5).
*Source: X2; journey steps 2, 5; R4; fresh-eyes S5.* · *Evidence: research (streak loss), role-play (R4).*

**US-10 Come back after a few days** · Must
As a returning creative, I want the app to open on today after a gap so that I can just carry on.
- [ ] After any gap under 14 days, the app opens on the normal, calm Today screen (US-08). **No welcome-back line**: noticing the gap is itself a gap count (S4).
- [ ] It doesn't ask me to explain or fill in the gap; yesterday can still be logged (US-05).
*Source: decision "comeback is a core flow"; journey steps 5–6; fresh-eyes S4 (5/5).* · *Evidence: research (fresh-eyes), past (irregular writing).*

**US-11 Come back after a missed week** · Must
As a returning creative, I want to choose how to continue after a week away so that I never have to start over unless I want to.
- [ ] After **14 days with no activity of any kind** (any tap counts), a **dismissible card on Today** (not a blocking screen) offers two choices: **pick up where I left off** or **join the current week**, as two equal cards (layout reference: Runna, C4). Neither is styled as the "right" one; no "missed" wording.
- [ ] Shown once per gap; dismissing it keeps the current week.
- [ ] What each choice does to the week number, day 7 and week 12 follows the time model (S3).
- [ ] **Start again from week 1** is available as a secondary option (e.g. a text link), never a primary button or default.
- [ ] One sentence of inspiration, our own words.
- [ ] The word "pause" isn't used in a way that reads as "wait until you're ready" (R7).
*Source: decisions on missed week (2026-11-15, 2026-11-27); journey step 8; R7; fresh-eyes S4.* · *Evidence: past, role-play (R7), decision (14-day threshold; the paper prototype's days-written count may move it).*

## E4. The pattern view
**US-12 Ideas first** · Must
As a returning creative, I want the pattern view to lead with my recurring ideas so that I see what keeps calling me, not just what I already know.
- [ ] The top of the pattern view shows ideas, with recurring ones grouped **by the links I've confirmed** (US-28) and counted plainly (e.g. "came up 3 times").
- [ ] Each idea shows its context: how the pages felt that day, the themes around it, and where it came from (after pages, after a date, on its own).
- [ ] Ideas written after a heavy page can be seen as such; any link between heavy pages and ideas is shown only as a plain count with its base ("6 of 9"), never as a cause or a headline.
- [ ] Recurring themes come after, as context. **No mood timeline** (S6).
*Source: decision "pattern view leads with ideas"; journey step 7a; R6; fresh-eyes S6.* · *Evidence: past (goal: creative direction), role-play (R6), research (fresh-eyes 5/5 on mood bias).*

**US-13 Useful with little data** · Must
As a returning creative, I want the pattern view to make sense with only a few irregular notes so that week 5 isn't a disappointment.
- [ ] The pattern view is **text-first at every data level**: a plainly counted list is the main form; charts, if any, are secondary (C2).
- [ ] With fewer than 5 captures it shows only a plain **"so far" list** of my ideas and themes. This list belongs to US-13, so cutting US-15 never breaks it (S9). *(5 is provisional; the paper prototype sets it, see `research/paper-prototype.md`.)*
- [ ] Weeks 1–2: visible, with a calm empty state and no pushed insights.
- [ ] No wording ever suggests writing more or differently to get "better" patterns (Q4 writing for the tag).
*Source: decision "pattern view low-key in weeks 1–2"; journey step 7a; walkthrough C2.* · *Evidence: research (book's no-rereading advice), role-play (C2).*

**US-14 Merge themes** · Must
As a returning creative, I want to merge themes that mean the same thing ("работа" + "work") so that writing in two languages doesn't split my patterns.
- [ ] I can merge two or more themes and pick the name that shows.
- [ ] A merge can be undone.
- [ ] Future suggestions use the merged theme.
*Source: decision "bilingual notes with manual merge".* · *Evidence: past (I write in both languages).*

**US-28 Link the same idea** · Must
As a returning creative, I want to mark two ideas as the same idea, even in different words or languages, so that "recurring" means what keeps coming back to me.
- [ ] In the pattern view, I can link an idea to an earlier one ("same idea as…"), and unlink it.
- [ ] **Optional AI suggestions (S1b):** off until I turn them on. When on, in the pattern view or the check-in (never in the capture), AI looks only at my idea text and proposes pairs ("these look like the same idea, link them?"). One tap confirms or rejects.
- [ ] Nothing counts as recurring until I confirm the link.
- [ ] AI never summarises, interprets, reads moods, themes or notes, or touches the pages; it only proposes pairs.
- [ ] If AI is off or fails, manual linking works the same.
- [ ] Linked ideas show under one name I choose, with every original wording kept.
*Source: fresh-eyes A1 (5/5), S1, S1b; positioning "AI connects your own ideas" (2026-11-27).* · *Evidence: research (fresh-eyes), past (bilingual notes).*

**US-15 "So far" recap, any time** · Should
As a returning creative, I want a recap of my progress, moods and ideas so far, open any time, so that insight counts whenever I stop.
- [ ] A recap mode of the pattern view, available from day 1 (the plain "so far" list itself is in US-13).
- [ ] Progress is plain numbers of what I made only (weeks, ideas, artist dates, notes); **no page days**, percentages or targets (X2, S5).
- [ ] Moods are shown only as context for ideas; never as a series, never interpreted or diagnosed (S6).
*Source: decision "always-available recap" (2026-11-27); success = insight; fresh-eyes S5, S6, S9.* · *Evidence: decision.*

**US-16 Accessible patterns** · Must
As a returning creative using a screen reader or without color, I want every pattern available as text so that nothing depends on seeing a chart.
- [ ] Every chart has a text equivalent (covered by default: the counted list is the main form, C2); moods are never color-only.
- [ ] Long lists have headings and grouping a screen reader can navigate.
*Source: brief accessibility criteria.* · *Evidence: research (WCAG).*

## E5. Artist dates
**US-17 Plan an artist date** · Must
As a returning creative, I want to plan a small artist date so that it fits a week with work and kids.
- [ ] Plan is optional text and an optional day; no time slot required.
- [ ] Suggestions are small (about 30 minutes, possible at home) and span my media (drawing, writing, photo, crafts, singing, video). Our own content.
- [ ] Weeks 1–4: suggestions lean toward permission ("small counts").
*Source: brief; persona (permission, time, kids); journey step 2.* · *Evidence: past, research (practitioners).*

**US-18 Idea → artist date** · Should
As a returning creative, I want to turn one of my ideas into my next artist date in one tap so that recurring ideas turn into something I do.
- [ ] Each idea in the pattern view has "Make it my next artist date".
- [ ] The plan opens prefilled with the idea's text, editable.
- [ ] The date stays linked to the idea.
*Source: decision 2026-11-27; journey step 7b.* · *Evidence: decision, role-play (7b).*

**US-19 Mark a date done + what came out of it** · Must
As a returning creative, I want to mark a date done and note what came out of it so that I see what my practice produces.
- [ ] Done is one tap; the note is optional, one sentence, text only.
- [ ] In the pattern view the note appears next to the idea it came from, if any (idea → date → what came out).
- [ ] A week with no date is shown neutrally, with no "missed" state.
- [ ] An idea that comes out of a date can be saved as an idea marked "after an artist date" (US-27).
*Source: decision "what came out of it?" note; US-18.* · *Evidence: decision.*

## E6. The week and the course
**US-20 Day-7 check-in** · Must
As a returning creative, I want an invited check-in on my day 7 that shows me what surfaced so that I notice patterns without being graded.
- [ ] Invited on day 7 of my week; can be dismissed; the next week opens either way (weeks never lock).
- [ ] The artist date is **prefilled** from my taps; nothing is asked twice.
- [ ] It **leads with what surfaced** (recurring ideas, themes, links); counts come after, small and neutral, and only of what I made (ideas, dates, notes), **never page days** (R3, S5).
- [ ] If AI idea links are on, new suggestions can be confirmed here (US-28).
- [ ] If I don't open it on day 7, it stays open until the next week's check-in; check-ins never stack (S3).
- [ ] A missing artist date: one neutral line + one small, at-home suggestion.
- [ ] One optional reflection line, our own wording.
- [ ] Takes **under 2 minutes**.
*Source: check-in decisions; decision "weekly patterns in the day-7 check-in"; journey step 4; R3; fresh-eyes S3, S5.* · *Evidence: decision, role-play (R3).*

**US-21 Help resources, only if I choose** · Should
As a returning creative, I want to decide whether the app ever shows help resources so that it never acts like a mental-health tool unless I ask.
- [ ] Off by default; turned on in settings.
- [ ] When on, a quiet link appears on heavy days; never a pop-up.
- [ ] (The one static help line in Settings is part of US-26, so it stays even if this story is cut.)
*Source: decision 2026-11-21 (heavy-day "never" list).* · *Evidence: decision.*

**US-22 Light 12-week path** · Must
As a returning creative, I want to see which week I'm in and its theme so that I feel the course frame without homework.
- [ ] Current week number and a short theme in our own words (never the book's theme names); all 12 weeks visible, none locked.
- [ ] No weekly task lists.
- [ ] Which week is "current" follows the time model (S3).
*Source: brief; weekly tasks parked; fresh-eyes S8 (copyright).* · *Evidence: decision.*

**US-23 Early support, weeks 1–4** · Must
As a returning creative, I want extra permission and calm in the first weeks so that I get past where I've stopped before.
- [ ] Weeks 1–4 show short permission framing in the places above (capture, check-in, artist date): on in weeks 1–4, off from week 5 (no week-by-week tapering in v1, S9).
- [ ] From week 5 it's gone; a heavy day still gets the US-07 line, without "early".
*Source: decision "early support weeks 1–4"; fresh-eyes S9.* · *Evidence: past (both attempts ended in weeks 1–2), research (practitioners stall in weeks 2–5).*

**US-24 Course complete** · Must
As a returning creative, I want a closing moment after week 12 that looks back at what surfaced so that the course has an ending.
- [ ] Shown once after week 12; reopenable.
- [ ] Leads with recurring ideas and what my dates produced (idea → date → what came out), not stats (uses US-15).
- [ ] Then one optional question: which idea do I want to keep going with? Picking one (or none) is one tap.
- [ ] After the course, the chosen idea is the first thing I see; "Pages done", capture and the pattern view keep working. Nothing locks or disappears.
- [ ] The formal ending is for week 12 only; stopping early is covered by the "so far" recap (US-15), with no "the end" screen.
- [ ] No confetti-style celebration unless I decide otherwise in Phase 4.
- [ ] Built around week 8 of my real use, with real data (S9).
*Source: brief; journey step 10; decision 2026-11-27 (ending = look back + one idea to carry forward).* · *Evidence: decision (no evidence past day 10).*

## E7. My data
**US-25 Saved between visits** · Must
As a returning creative, I want my logs and notes to persist so that weeks of patterns are never lost.
- [ ] Data survives closing the app, reloading and coming back weeks later.
- [ ] One "Download my notes" control in settings saves a plain text/CSV file: dates, moods, themes, ideas, artist dates and their notes.
- [ ] Export only; no import in v1 (parked for v1.1).
- [ ] Data lives in the artifact's saved data; the Phase 5 spike checks that the home-screen icon and the notebook QR open the same data, logged in.
*Source: brief; X3; decision 2026-11-27 (export only); fresh-eyes A6.* · *Evidence: decision.*

**US-26 Settings** · Must
As a returning creative, I want one calm place for the few things I set so that nothing important is hidden.
- [ ] Change my start date (with a plain note on what it changes, per the time model).
- [ ] Show the notebook card again (US-03).
- [ ] Help resources on/off (US-21), plus **one static help line that is always there**, off or on.
- [ ] AI idea links on/off (US-28), with one line on what is sent (only idea text).
- [ ] "Download my notes" (US-25).
- [ ] **Delete all my data**, with a plain confirmation that offers to download first.
*Source: fresh-eyes A12, A17, S11.* · *Evidence: research (fresh-eyes 4/5).*

---

## Not in v1 (see `ideas.md`)
"New pattern" card · Bulgarian UI · import from export file (v1.1) · letter to future me · AI shapes my ideas (v1.1) · app lock · mood timeline · linking patterns to my creative goal · reminders · AI handwriting scan · photos for date notes · weekly tasks · share card (v1.1).
*(The testers' demo copy moved to Phase 5, S12.)*

## Open questions
1. ~~**Export (US-25):**~~ ✅ decided 2026-11-27: keep (Must), export only; import parked for v1.1.
2. ~~**Priority cut line:**~~ ✅ decided 2026-11-27: if the build runs long, cut US-21 → US-15 → US-18 (US-18 last).
3. ~~**US-13 threshold:**~~ ✅ decided 2026-11-27: 5 captures, provisional; the paper prototype (started 2026-11-27) sets the real number.
4. ~~**US-24:**~~ ✅ decided 2026-11-27: a look back, then one idea to carry forward; the app keeps working after week 12. "Letter to future me" parked in `ideas.md`.
