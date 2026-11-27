# Fresh-eyes review: Artist's Sketchbook (end of Discovery)
*Reviewer 2 (accessibility, inclusive design). Read only brief, persona, journey, stories.*

## 1. Verdict in 3 lines
- **Right product, wrong data model:** a paper-first, no-judgment mirror fits a low-energy, guilt-prone returner well. But the stories still assume someone who writes daily, and she writes "when she needs to unload".
- **Biggest bet:** that self-named *ideas* will show recurring patterns (US-12) she can't see on paper.
- **Biggest risk:** ideas can only be logged after a pages tap, and nothing groups free-text ideas. The hook, then, will be sparse, skewed toward heavy days, and never "recur".

## 2. Top 5 problems
**1. "Recurring ideas" has no mechanism.** US-12 promises "came up 3 times", but ideas are free text (US-06) and merging exists only for themes (US-14). "Film the street at dusk" and "dusk video" will never match, and the brief rules out AI. *Why it matters:* this is the Must that journey 7a/R6 says will save the product. *Suggestion:* at capture, offer her past ideas as tappable chips ("this one again"). Each tap increments that idea. Write this into US-06/US-12 as acceptance criteria.

**2. Ideas are gated behind "Pages done".** US-06 says the capture appears "only after" the pages tap. Yet persona "Daily context" says she writes only on emotional need and opens the app whenever she remembers. *Why it matters:* the hook (ideas) depends on her least frequent behavior (pages), and the sample is biased toward heavy days. The "ideas cluster on heavy days" finding in journey 7b could simply come from *when* she's allowed to log. *Suggestion:* add a Must story, "Add an idea" from Today on any day, with no pages tap needed, and mark each idea with its origin (after pages / after a date / standalone).

**3. Counting returns through the back door.** X2 and R4 ban gap counts. Yet the brief's check-in prefills a "pages count", US-20 shows counts "small and neutral", US-15 shows "page days", and journey 4 has her thinking "Three pages days and no date". A page-day count inside a 7-day frame *is* a gap count (3 means 4 missing). *Suggestion:* drop page-day counts from the check-in and the recap. Count only what she *made* (ideas, dates, notes).

**4. Comeback triggers will fire on her normal rhythm.** US-10 fires after "2+ days without a log" and US-11 after "7+ days". For someone who writes irregularly, a 2-day gap is the norm, so "welcome back" becomes the line she sees most often. That line itself tells her she was away, which is a softer gap count. US-11 then blocks her with a choice screen at her most avoidant moment (journey 8: −2). *Suggestion:* no trigger-based copy for short gaps; Today always looks the same. For the missed week, show the choice as a quiet inline card on Today, dismissible, and default to the current week. Don't use a blocking screen.

**5. The week/day state model is undefined.** The brief's core loop says "the path moves on with the calendar". US-11 offers "pick up where I left off", which detaches week number from date. Once that happens, what decides US-20's "day 7", US-22's current week, US-23's week 1–4 tapering and US-24's "after week 12"? *Why it matters:* every Must in E6 depends on it. *Suggestion:* write a one-page state model before flows: course week vs calendar date, what "pick up" shifts, and the day boundary (a 1 a.m. kitchen session belongs to which day?).

## 3. What's strong
- **The wordless "heavy" option plus room-first copy (US-07, R1, R2).** It correctly treats naming the feeling as the barrier (persona Q2).
- **US-08 "Nothing to log today" as a designed, complete state.**
- **Text-first pattern view at every data level (US-13, US-16, C2).** It solves screen-reader access and sparse data in one move.
- **Evidence tagging.** The persona is honest that everything past day 10 is unknown.

## 4. What's missing
- **Storage durability.** In browser storage, iOS Safari can evict data from an uninstalled web app after about 7 days of non-use, which is exactly this user's missed-week case. US-25 says "survives coming back weeks later" with no plan for it. Requiring home-screen install, requesting persistent storage, and adding a gentle export prompt need to be Must-level.
- **A settings screen.** US-03, US-21 and US-25 all point to "settings", but no story defines it (start date, card, resources, export, delete all).
- **Backfill beyond yesterday.** US-05 blocks it, but her notebook is dated. Opening on day 3 means a real page can never be captured. Blocking loses data and implies "those days are gone". Consider a secondary "an earlier page" option for captures only.
- **The mood set itself.** Count, words, fixed or custom: unspecified, though US-12 and US-15 depend on it.
- **Privacy on a shared family phone** (persona: kids). There's no app lock or discreet mode, and heavy-day notes are sensitive.
- **Undo for deleting a capture**; multiple ideas from one page.

## 5. Scope
- **Cut:** the "shorter pages" option in US-04. It creates a full/short hierarchy, which is a judgment, and the persona asks only that short mornings *count*. If everything counts, the distinction is noise.
- **Demote to Should:** US-24 (course complete). There's zero evidence past day 10 (journey stage E). Build it last; US-15 already carries "insight counts whenever I stop". Also US-23's *tapering* logic: static early-weeks copy is enough for v1.
- **Merge:** US-02 into US-01 (an onboarding step).
- **Fix the cut order:** US-15 and US-18 are "first to cut". But US-13 falls back to the "so far" list (US-15), and US-19/US-24 (Musts) depend on the idea → date link (US-18). Cutting them breaks Musts. Either promote them or rewrite the dependents.
- **Absent Musts:** standalone idea capture (problem 2), idea recurrence linking (problem 1), storage durability, settings.

## 6. Contradictions
- **US-07:** "without needing a word for the feeling" vs "every mood option is an icon + a word". Clarify that the label names the *weight*, not the emotion.
- **Brief/US-07:** the heavy-day line says an *early* dip is normal, while US-23 keeps it after week 5. In week 9 that copy is wrong.
- **Brief:** "low-key in weeks 1–2, no pushed insights" vs US-20/journey 4, where the day-7 check-in pushes the week's patterns in week 1. US-15 also shows a recap from day 1.
- **Brief:** "morning pages every day" as the premise vs persona: writes only on need. The product hasn't decided which user it's for.
- **Core loop "path moves with the calendar"** vs US-11 "pick up where I left off".
- **Journey 7a:** "tired" listed as a theme; it's a mood. If the designer blurs them, so will the user.

## 7. Accessibility & wellbeing risks
- **Mixed-language notes:** a Bulgarian note inside an English UI will be read with English pronunciation unless the text is tagged with its language (WCAG 3.1.2). Detect Cyrillic and set `lang="bg"` per note.
- **The "10 s capture" is unrealistic for two free-text fields** with a keyboard switch to Cyrillic, typed one-handed (X5). For motor or low-energy states, make chips (past entries) the main path and typing the fallback. Suggestion lists need proper combobox semantics and announced result counts.
- **A mood-over-time view for a release-valve writer will be mostly "heavy".** That's a self-portrait of distress she didn't ask to see, and it contradicts the role-play ("I'd close the app"). Consider no default mood timeline; show mood only as context per idea.
- **Help resources are off by default *and* first to cut (US-21).** Fine for n = 1, but the case study needs one quiet, always-reachable line in settings even with the toggle off.
- **Mood icons are ambiguous:** the word carries meaning; mark icons `aria-hidden`.
- **Undo for "Pages done"** must be reachable without a time-limited toast (WCAG 2.2.1); a persistent "undo" on Today avoids a timing trap.
- **No story covers an announced "done" confirmation** that works without animation or color (WCAG 4.1.3).

## 8. Questions I'd ask the designer
1. If you only write when you need to unload, what share of your ideas actually arrive *after pages*, and what does the paper prototype show so far?
2. How should two differently worded ideas become "the same idea" without AI, and would you do that linking yourself?
3. Is a page-day count in the check-in something you want, or something the course structure assumed?
4. When you "pick up where you left off", what date is your day 7?
5. Who else picks up your phone, and would you be comfortable with them seeing a heavy-day note?
