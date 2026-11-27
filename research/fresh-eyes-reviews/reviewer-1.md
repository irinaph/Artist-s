# Fresh-eyes review: Artist's Sketchbook (end of Discovery)

## 1. Verdict in 3 lines
Mostly the right product. "Paper stays paper, the app keeps your own small notes" fits someone who writes only when she needs to unload, though the 12-week course spine fits her less well than the docs assume.
Biggest bet: optional, free-text *ideas* will recur often and match closely enough for a rule-based pattern view to show her something new.
Biggest risk: irregular writing plus optional fields means too little idea data by week 5, and nothing in the stories can tell that two differently worded ideas are the same idea.

## 2. Top 5 problems

**1. "Recurring ideas" can't be detected as specified.**
- *Evidence:* US-12 counts recurring ideas and journey 7b imagines one recurring 4 times. But ideas are free text (US-06), there's no AI (brief), and merge exists only for themes (US-14).
- *Why it matters:* "film the street at dusk" and "dusk video" never match, so the headline feature (R6) becomes a list of one-offs.
- *Suggestion:* when she saves an idea, offer her past ideas as "same as…" links, or let her star ideas to keep circling. Make this a Must and demote US-14 if you need the room.

**2. Ideas can only be entered after "Pages done".**
- *Evidence:* US-06 shows the capture "only after" Pages done. The persona writes only when she needs to (Daily context), and her goal is creative direction (Goals 2).
- *Why it matters:* the hook is gated behind her least reliable practice. Ideas from an artist date or a commute are lost.
- *Suggestion:* add a standalone "Add an idea" entry on Today, with no pages required.

**3. Sparse data is designed for but not counted.**
- *Evidence:* journey 7a assumes about 12 captures by week 5. The success criterion asks for one new pattern after 2 weeks, while US-13 hides patterns below 5 captures and keeps weeks 1–2 low-key.
- *Why it matters:* at 2–3 writes a week, mostly mood-only, the 2-week criterion is impossible by design, so you'll read a spec artefact as product failure.
- *Suggestion:* set the thresholds from the paper prototype's real fill rate per field, and restate success as "N ideas with context by week X".

**4. "Missed week" is her normal week.**
- *Evidence:* US-11 fires after 7+ days without a log, but she writes "when she feels the emotional need". US-05 also blocks backfill older than yesterday, even though her notebook is *dated*.
- *Why it matters:* the exception flow becomes routine, and keeps reminding her of a pace she isn't keeping. Blocking backfill throws away real entries she could copy from paper, which starves problem 3.
- *Suggestion:* trigger US-11 on course-week change, not on days without a log. Add an unprompted "add an earlier page" limited to the current week.

**5. Role-play has become requirements.**
- *Evidence:* the journey says to treat [role-play] like [assumption], yet R1–R7 are now Must criteria (US-07, US-08, US-11, US-12, US-20). Persona quit reasons Q5–Q6 name the designer-as-user bias, and the only mitigation is a demo copy (journey 9).
- *Why it matters:* an agent playing a persona the designer wrote about herself is a closed loop. The case study will read as self-confirming.
- *Suggestion:* tag every Must criterion with its evidence level, and name which R-findings the paper prototype must confirm before flows lock.

## 3. What's strong
- **The positioning is a real gap:** paper first, she names her own tags, nothing is read.
- **The heavy-page moment (US-07, journey 3):** a wordless "heavy" option, one line of copy, an optional follow-up, and no patterns in that moment.
- **No gap counts anywhere (X2, US-09), extended to the paper card (US-03):** the dread starts before the app opens.
- **The "nothing to log today" state (US-08):** a commonly missed state, named as core.

## 4. What's missing
- **A settings story.** US-03, US-21 and US-25 point to settings, but nothing defines it: changing the start date, deleting all data.
- **Storage durability.** With no account (X3), data lives in browser storage, which iOS can clear after a period without use. That's the gap scenario, and the export (US-25) is manual. Request persistent storage, and add a quiet backup nudge.
- **Shared-phone privacy.** She has kids, and heavy-day notes sit in an unlocked web app. Consider an optional lock or a discreet icon and name.
- **The day-7 check-in when she doesn't open the app on day 7.** Does it wait, expire, or merge into the next week?
- **Edge cases:**
  - The midnight boundary for "yesterday".
  - Two artist dates in a week, or a date with no pages that week.
  - Editing or deleting a planned date.
  - What "pick up where I left off" does to week numbering and to which day is day 7.
- **The mood scale.** Only "heavy" is specified. And is "how the pages felt" over time (US-12, US-15) meaningful as a mood trend?
- **What replaces early support after week 4 (US-23).** No story covers it.

## 5. Scope
- **Demote US-24 to Should and build it in week 8 of real use.** She has never passed day 10, and by then there will be real data to design the look back from.
- **Merge US-15 into US-13.** "So far" means two different things (a fallback for thin data and a recap mode).
- **Demote US-14 to Should** if idea matching takes its slot.
- **US-03 is a Must, but it's content, not build.**
- **Absent Musts:**
  - Idea matching (problem 1).
  - Standalone idea capture (problem 2).
  - Durable storage and backup.
  - Settings, including deleting all data.

## 6. Contradictions
- **When the path moves.** Brief core loop: "the path moves on with the calendar". Brief decision: "pause the path or continue". US-11: "pick up where I left off". Three models of week time.
- **The 2-week pattern.** The success criterion wants a new pattern after 2 weeks. The brief and US-13 keep weeks 1–2 low-key and hide patterns below 5 captures.
- **"An early dip is normal" after week 4.** US-07's line survives past week 5 (US-23). At week 9, "early" is false.
- **Counts vs X2.** X2 bans gap counts, yet US-20 and US-15 show "page days". In a 7-day check-in, "3" reads as 3 out of 7, which is exactly the role-play's reaction in journey 4.
- **Mood: now or then?** Persona decision 1 still lists "mood while writing vs now" as an open sub-question. US-06 has settled it silently.
- **Who the success criteria are for.** The persona calls them the project's goals, not hers. The brief already lists 6 weeks of insight as the main criterion, so the persona's caveat is out of date.

## 7. Accessibility & wellbeing risks
- **The wordless "heavy" option still needs a spoken label,** and an icon that isn't a colour or facial nuance (X1, US-07).
- **Bulgarian notes need `lang="bg"` when shown,** or screen readers pronounce Cyrillic with English rules. X4 omits this.
- **Text-first lists (US-13, US-16) will get long.** Plan headings and grouping so a screen-reader user can navigate them.
- **Showing ideas "after a heavy page" can romanticise distress** (US-12, journey 7b: "most ideas came on heavy days"). Frame it neutrally, and never present it as a pattern to repeat.
- **No safety net by default.** Help resources are off by default (US-21), and anger is a documented trigger. Fine for n = 1 by her choice; a blocker before any tester.
- **A run of heavy entries will show in "moods over time"** with no defined behaviour. Decide it deliberately: no escalation, and no accidental silence.

## 8. Questions I'd ask the designer
1. How many captures, and how many idea fields, did the paper prototype actually produce?
2. At two or three writes a week, is the 12-week course still the spine, or is this an idea journal that knows about the course?
3. Without AI, how does the app know two ideas are the same idea?
4. Where does the data physically live, and what happens if the browser clears it or you lose the phone?
5. Who other than you (or an agent playing you) will test the R-findings, and which would you drop if the prototype contradicts them?
