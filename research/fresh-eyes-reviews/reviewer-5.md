# Fresh-eyes review: Artist's Sketchbook (end of Discovery)

## 1. Verdict in 3 lines
Right product for this persona, but it's still shaped like a daily morning-pages tracker for someone who writes only when she needs to unload and came for her ideas.
Biggest bet: a few optional, free-text, bilingual notes will show a recurring idea she couldn't see on paper (US-12, and the 2-week success criterion).
Biggest risk: data. Sparse captures, free-text ideas that can't be grouped, and browser storage that may lose or split her data during the gaps the product is built around.

## 2. Top 5 problems

**P1. The core feature, "recurring ideas", has no grouping rule and no data model.**
Evidence: US-12 ("recurring ones grouped and counted"); journey 7b ("4 times across weeks"); US-14 offers merge for *themes* only.
Why it matters: ideas are free-text sentences in two languages, so "film the street at dusk" and its Bulgarian version will never match. Without a rule, US-12 is a list of one-offs, which is exactly the 7a failure. It's also the largest unknown in the build.
Suggestion: group at capture time. When she saves an idea, offer "same as an earlier idea?" with her past ideas (the US-06 suggestions already exist). The count then comes from a link stored with each idea, with no text matching needed. Extend US-14 merge to ideas as the fallback.

**P2. The product optimises the tap, but her value is in the idea field.**
Evidence: brief Constraints ("#1 build constraint"); persona Daily context ("writes when she needs to"); journey insight 5 ("ideas, not moods").
Why it matters: with no streaks or gap counts (X2, US-09), "Pages done" gives her almost nothing back. It's a gate in front of the capture. And ideas also come after artist dates, during the day, or on days with no pages, and the model can't record those.
Suggestion: add a Must, "capture an idea any time, without pages". Keep the 5 s tap, but make the #1 constraint "an idea is saved within 10 s of tapping the home-screen icon".

**P3. Storage can quietly destroy the 12-week dataset.**
Evidence: X3 "no account"; US-25 export with no import; US-03 QR card; US-02 shortcut.
Why it matters: on iOS, a home-screen web app and Safari keep separate storage. Scanning the notebook QR opens Safari, which is a second, empty copy of the app. Safari can also clear stored data for sites she hasn't opened in about 7 days, which is her US-11 case. An export with no import is not a backup.
Suggestion: make persistence a Phase 3 Must. Options: a tiny backend with a passphrase, or install-only plus `navigator.storage.persist()`. Point the QR at an "open your installed icon" page. Move import from v1.1 into v1.

**P4. The time model is undefined after a gap.**
Evidence: US-11 "pick up where I left off" vs "join the current week"; US-20 "day 7 of my week"; US-10 "2+ days without a log"; US-22; US-24.
Why it matters: "pick up" pulls course weeks apart from calendar weeks. Then when is the check-in, what does US-22 show, and when is "after week 12"? For someone who writes irregularly, a 7-day gap is ordinary, so US-11 fires often and turns a normal week into a decision. It's also unclear what counts as "a log": pages, a capture, a date, or just opening the app (US-08)?
Suggestion: specify `start_date + offset_days → current_week`. Count any capture or date as activity. Trigger US-11 only after 10–14 days.

**P5. 20 of 25 stories are Must, which is too many for one person to build before her own day 1.**
Evidence: priority tags; the cut line names only US-21, US-15 and US-18.
Why it matters: a half-built app on day 1 turns using it into testing it (Q5/Q6).
Suggestion: build a thin slice for week 1 and add the later-week features while she's in the early weeks (section 5).

## 3. What's strong
- **X2, US-09 and R4 ("no gap count, however kindly worded")** are rules you can fail a build on, and they're the real differentiator against the competitors in the brief.
- **R1, the wordless "heavy" option (US-07)**, comes from where attempt 2 actually ended.
- **The text-first pattern view (US-13 C2, US-16)** solves accessibility, sparse data and build cost with one decision.
- **Honest evidence tagging.** Weeks 3–12 are openly marked as having no evidence, and role-play is kept separate from evidence.

## 4. What's missing
- **Idea capture without pages**, and ideas from artist dates going into the same idea pool.
- **Backfilling from the dated notebook.** US-05 blocks anything older than yesterday, so real entries from gap days are lost. Offer it as an option that is never prompted.
- **Day boundary.** Which day does a log at 00:30 count for, and what does "yesterday" show if yesterday is already logged?
- **A Settings story.** US-03, US-21 and US-25 all point into Settings, and none defines it: changing the start date, deleting all data, and the demo copy (which Q6 needs during real use, not in Phase 7).
- **A missed check-in.** If she opens the app on day 9 and the check-in never happened, does it roll forward? Does it stack with the US-10 welcome-back?
- **Artist-date edges:** two dates in a week, a date planned and never done, a date made from an idea and then edited (does the US-18 link survive?).
- **The US-04 "shorter" flag.** No story consumes it.

## 5. Scope
- **Cut:** the US-04 "shorter" toggle. Nothing reads it, and it labels a lesser day.
- **Still v1, but not day-1 Musts:** US-24 (build it by week 8), US-11 (by week 2), US-14 (by week 2), US-23's tapering (static week-1 copy first).
- **Demote to Should:** US-02's install tutorial (one line will do) and US-03 as a printed QR card.
- **Keep US-18:** it's the only story that turns a pattern into action (7b).
- **Missing at Must level:** idea capture without pages (P2), persistence plus import (P3), idea grouping (P1), and the time model (P4).

## 6. Contradictions
- **The brief's success criterion** ("a pattern I didn't notice after 2 weeks") vs US-13 (low-key in weeks 1–2, a threshold of 5 captures) and a persona who may log only 4 times in two weeks.
- **Brief Decisions ("pause the path or continue")** is stale against US-11 and R7.
- **The brief's core loop opens "Morning: write pages"**, while the persona says the pages have no fixed time.
- **US-07's "an early dip is normal"** is the line US-23 keeps after week 5, so in week 9 she'd be told her dip is "early".
- **US-15 shows "page days" as plain numbers.** In week 6, "3 page days" is a gap count by subtraction, which X2 forbids. Journey step 4 even has her reading "three pages days".
- **US-01 says "at most 2 screens"**, but onboarding also holds the US-02 guide and the US-03 card.
- **Journey 7b celebrates "most ideas came on heavy days"**, while US-15 says moods are never interpreted.

## 7. Accessibility & wellbeing risks
- **Bilingual autocomplete (US-06, US-14)** needs a correct screen-reader combobox with matching across Latin and Cyrillic. It's the hardest widget in the app, so budget for it.
- **The wordless "heavy" option** still needs an accessible name. Test what VoiceOver reads for it.
- **A pattern view dominated by heavy moods.** She writes mainly to unload, so the recap (US-15) may be mostly heavy. That's a report card on her emotional life. Let her hide moods.
- **Distress as material.** "Ideas come on heavy days" can teach her that anger is productive. Show it as context, never as a headline.
- **Self-surveillance.** This is a designer studying her own moods in her own app (Q6). The demo copy belongs in v1.

## 8. Questions I'd ask the designer
1. If an idea comes to you during an artist date, where does it go now?
2. Who decides that two ideas are "the same idea", and when?
3. Where does your data live on your iPhone after you scan the QR on day 9?
4. After "pick up where I left off", which week are you in, and when is your check-in?
5. How many captures do you realistically expect in 14 days, and does the 2-week success criterion survive that number?
