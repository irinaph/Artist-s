# Reviewer 3: fresh-eyes review (behaviour change / wellbeing lens)

## 1. Verdict in 3 lines
**Right product, wrong unit of record:** "help me see what my creative mind keeps returning to" fits her, but every story hangs off a daily "Pages done" event she mostly doesn't produce.
**Biggest bet:** that 10 s of self-labelling on irregular days builds an idea pattern she couldn't see on paper (US-12, US-13).
**Biggest risk:** calendar-driven gap signals that nobody designed as gap signals (welcome-back lines, missed-week choices, week numbers, page-day counts) bring back the R4 dread through side doors.

## 2. Top 5 problems

**P1. Ideas can only be logged after "Pages done", yet ideas are the product.**
*Evidence:* US-06 says the capture comes "only after Pages done". R6 and US-12 make ideas the headline. The persona writes "when she feels the emotional need".
*Why it matters:* a multi-passionate creative gets ideas in the car or mid-artist-date. Locking them behind a pages event starves the pattern view.
*Suggestion:* a Must story, "capture an idea any time". Record where the idea came from (after pages, after a date, standalone) as metadata, not as a precondition.

**P2. "Recurring ideas" has no mechanism.**
*Evidence:* US-12 promises ideas "grouped and counted", but US-14 gives merge to themes only, and ideas are one-off sentences.
*Why it matters:* free-text ideas almost never repeat word for word, so every count is 1 and journey step 7b never happens. The core value proposition has no acceptance criterion.
*Suggestion:* decide before the flows: a "same idea as…" link at capture (suggest past ideas, as US-06 does for themes). Make it Must, and test it in the paper prototype.

**P3. Sampling bias will produce false insight.**
*Evidence:* she writes to unload. US-07 tags ideas "after a heavy page". Journey 7b expects the finding "most ideas came on heavy days".
*Why it matters:* if she mainly writes on heavy days, most captures are heavy by construction. The app would "discover" an artifact of when she writes. "Your ideas come from pain" is a loaded thing to be told by a chart.
*Suggestion:* show co-occurrence with the base rate ("6 of your 9 notes were after heavy pages"), never as an implied cause.

**P4. The comeback flows will fire constantly.**
*Evidence:* US-10 triggers at 2+ days, US-11 at 7+ days, and she writes irregularly.
*Why it matters:* at 2 to 3 pages a week, nearly every visit gets a welcome-back line, which is itself a gap message: the app noticed she was gone. US-11 could interrupt her several times over the course.
*Suggestion:* drop the US-10 line so that today simply opens. Ask US-11 at most once per course week. Specify what "pick up where I left off" does to the start date, the day-7 anchor and the week theme. That state model doesn't exist.

**P5. Counts reintroduce the scorecard.**
*Evidence:* US-15 shows "page days", US-20 has "counts come after", US-22 shows the week number.
*Why it matters:* "Week 6 · 9 page days" is a gap count once she does the subtraction, which X2 bans in spirit.
*Suggestion:* drop page-day totals. Count per idea ("came up 3 times"), never per day.

## 3. What's strong
- **Paper-first, "nothing is read unless you choose":** it respects the practice and fills a real competitive gap.
- **The US-07 heavy-day sequence:** a wordless option, one line, an optional "what's clearer now?", no cheering up, no patterns shown in the moment. Unusually well reasoned.
- **The evidence tags and the admission that weeks 6–12 can't be designed from evidence.** That honesty makes the case study credible.
- **US-08 "nothing to log" as a complete state.** This is the comeback that matters, and most habit apps never design it.

## 4. What's missing
- Standalone idea capture (P1) and idea grouping (P2).
- **The mood scale:** how many options, and what range? Every pattern depends on it, and nothing defines it.
- **Day-7 edge cases:** she opens the app on day 10, or two check-ins are pending after a gap. Is the invitation stale, stacked or dropped?
- **A planned date that isn't done at the week rollover:** does it carry over or disappear?
- **Logging after midnight:** is it "today" or "yesterday" (US-05)?
- **A shared phone:** she has kids. Themes like "my sister" and a row of heavy days are visible to anyone. There's no lock and no option to hide content.
- **Data loss:** no account plus export-only (US-25) means a lost phone or a browser storage purge after weeks of not using the app erases everything, and that's exactly her missed-week case. A backup you can't import isn't recovery.
- **Deleting an idea that's linked to an artist date** (US-18).
- **A testable definition of "real insight"** for the brief's success criterion.

## 5. Scope
**Demote or cut:**
- **US-24 → build during weeks 6–10.** She has never reached day 10, and it isn't needed until week 12.
- **US-14 → Should.** With about 12 captures, the US-06 suggestions already prevent most splits. Spend that effort on grouping ideas.
- **US-03 → a design deliverable, not a story.** It's a printed card with no software behaviour.
- **US-04 "shorter pages" option → cut.** It records quantity that nothing in the pattern view uses.

**Promote:**
- **US-15 → Must.** US-13's fallback for small data is the "so far" list, so cutting US-15 breaks a Must story.
- **US-21 → a minimal Must:** off by default, plus one static link always reachable in settings.

**Absent at Must level:** standalone idea capture, idea grouping, a defined mood scale.

## 6. Contradictions
- **The brief's success criterion,** "after 2 weeks… a pattern I didn't notice", conflicts with US-13 (low-key in weeks 1–2, only a list below 5 captures) and persona decision 6 (detection from week 3).
- **Brief "Decisions so far"** still says "pause or continue". US-11 and journey step 8 rejected "pause".
- **The brief's core loop says "Morning: write pages",** while the persona says mornings vary, and US-04 bans "this morning".
- **The brief's feature table** puts "moods over time" first. US-12 leads with ideas.
- **US-07** says "heavy without a word for the feeling" but also "every option is an icon + a word". It works only if "heavy" is that word; state it explicitly.
- **US-22** says "theme in our own words", but the brief lists the course's theme names. Decide which one ships.
- **US-01** allows at most 2 screens in under a minute, while journey step 0 also puts home-screen setup (US-02) and the card (US-03) into onboarding.

## 7. Accessibility & wellbeing risks
- **The mood history as an emotional report card:** "moods over time" (US-12, US-15) makes heavy weeks visible as a record. Let her hide moods, and never chart heavy-day density.
- **Help resources are the first cut** (US-21) in an app that knowingly sits next to anger.
- **Bilingual output:** Bulgarian notes need a correct `lang` attribute, or screen readers mispronounce them. X4 covers input only.
- **The kitchen before dawn:** she needs a dark theme and a large, high-contrast "Pages done" target. X1 doesn't mention either.
- **The wordless "heavy" option** still needs a meaningful, non-clinical accessible name.
- **Builder-as-user (persona Q5/Q6):** this is the likeliest way the project fails. Move the separate demo copy to Phase 3.

## 8. Questions I'd ask the designer
1. In a typical week right now, how many days do you write pages? If the answer is 1 to 3, what is a "missed week" for you?
2. Where were you the last three times a creative idea came to you, and was your notebook with you?
3. At week 6, what exactly would you have to see on screen to say "real insight"?
4. Who else picks up your phone, and what would you mind them seeing?
5. Should the 12-week clock follow the calendar, or your pace?
