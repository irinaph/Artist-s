# Reviewer 4: content design / UX writing, fresh eyes

## 1. Verdict in 3 lines
Mostly yes. A paper-first reflection tool that collects ideas fits a lapsed, time-starved practitioner, but the course frame expects daily writing and the persona writes only when she needs to unload.
**Biggest bet:** irregular 10-second self-reports will surface a recurring *idea* she couldn't see on paper (US-12, journey 7b).
**Biggest risk:** the data will be sparse *and* weighted toward heavy days, so the pattern view could end up showing her mostly bad mornings and the same tags she typed before.

## 2. Top 5 problems

**1. The mood data is biased by when she writes, and nothing in the design accounts for that.**
*Evidence:* persona "Who she is" says she writes "only when she feels the emotional need"; the brief and US-12 both include "moods over time".
*Why it matters:* most captures will come from heavy days, so a mood timeline will read as a record of her low points. That is the "you've felt this way twice" moment that would make her close the app (journey 3 role-play), only spread over weeks.
*Suggestion:* drop the mood timeline from v1. Show mood only as a property of an idea ("came after a heavy page"), never as a series.

**2. Suggesting her past entries will make "recurring" partly an effect of the autocomplete.**
*Evidence:* US-06 ("suggest my own past entries"); persona quit reasons Q3 and Q4; US-12 ("came up 3 times").
*Why it matters:* reusing an old tag with one tap is the easiest action in a 10-second capture. Counts go up because the suggestion was there, not because the theme came back. That is the writing-for-the-tag risk built into the interaction, and it leads to Q3, where the patterns tell her nothing new.
*Suggestion:* suggest past themes but not past ideas. An idea is retyped or explicitly linked (problem 3).

**3. Nothing in the design groups ideas, yet the pattern view leads with recurring ideas.**
*Evidence:* US-12 requires "recurring ones grouped"; US-14 merges *themes* only; ideas are free text in two languages (US-06, X4).
*Why it matters:* "film the street at dusk" and "видео на залез" will never match as strings. The headline of the core screen depends on a mechanism no story describes.
*Suggestion:* add a Must story for manual idea linking ("same idea as…") at capture time or in the pattern view. Without it, US-12 can't pass its own acceptance criteria.

**4. The comeback copy breaks the "no gap shown" rule.**
*Evidence:* US-10 shows a welcome-back line after 2+ days; US-11 shows a screen after 7+ days; R4; US-09.
*Why it matters:* "Welcome back" tells her the app counted her absence. For someone who writes in bursts, 7+ quiet days are normal, so the missed-week fork will keep appearing and turn ordinary behaviour into a decision she has to make.
*Suggestion:* show no comeback line under 7 days; the US-08 Today screen *is* the comeback. At 7+ days, make "join the current week" the default and put "pick up where I left off" behind a quiet link.

**5. The heavy-day flow has a data-type problem.**
*Evidence:* US-07 saves the "what's clearer now?" answer as an idea; US-06 defines an idea as *creative*.
*Why it matters:* what surfaces after anger is often a life insight ("talk to my sister"), not a creative idea. Putting it in the idea list mixes the two in the ideas-first view and could put something private next to "Make it my next artist date" (US-18).
*Suggestion:* store it as its own note type. Let her promote it to an idea with one tap. Only promoted notes appear in US-12.

## 3. What's strong
- The evidence tagging is honest, and the role-play is explicitly not counted as evidence. Few portfolio projects do this.
- R1, the heavy option that doesn't need a word for the feeling, is a real content-design insight. Naming the emotion is the friction, not the tap.
- The check-in order in R3/US-20, showing what surfaced first with small neutral counts after, is the right hierarchy for a page about personal insight.
- US-08 designs a moment most apps leave out: opening the app and doing nothing is treated as a complete visit.

## 4. What's missing
- **Storage eviction:** a browser-tab web app on iOS can lose local data after a stretch of no use. For a user who has missed weeks, that could wipe the pattern view. US-25 doesn't cover it; US-02 is the real protection, so onboarding copy should say why to install.
- **What happens when several things are due on open:** check-in, missed-week choice and post-course idea (US-24) can collide with the US-04 5-second target.
- **Future start date (US-01):** what does Today show before week 1?
- **Pages written after midnight:** which day do they belong to?
- **An artist date done without a plan, or two in one week** (US-19).
- **A missed check-in:** can it be opened on day 9?
- **Restart from week 1** (US-11): what happens to the old patterns?
- **Notebook backfill:** US-05 blocks days older than yesterday, but the dated notebook has that data.
- **Privacy on a shared family phone**, and **delete all my data** (without it, X3 is only half covered).

## 5. Scope
- **Demote US-24 to Should.** Weeks 6–12 have no evidence (journey 9); build it during weeks 6–8 of real use.
- **Merge US-15 into US-13.** "So far" with fewer than 5 captures and a "so far" recap from day 1 are one screen with two names.
- **Simplify US-23.** Tapering week by week across three surfaces means 12 copy variants. Use on/off for weeks 1–4.
- **Cut US-21 as a feature.** She said never; keep one static line in settings instead.
- **Missing at Must level:** idea linking, a separate note type for heavy-day insights, delete all data, and a priority rule for what shows on open.

## 6. Contradictions
- **Brief Decisions** still says "pause the path or continue"; the brief's own MVP scope, journey 8 and US-11 replaced it.
- **The brief says no pushed insights in weeks 1–2**, yet the week-1 check-in leads with what surfaced (US-20) and the recap is available from day 1 (US-15).
- **The US-07 line says an early dip is normal**, and US-23 keeps it from week 5 on. In week 9 that isn't true.
- **US-07:** the heavy option needs "no word for the feeling", yet every option is "icon + a word". Spell out how a word for *weight* differs from a word for *emotion*, or R1 will get undone.
- **The brief names weeks by theme; US-22 says "our own words".** Decide which, partly for copyright reasons.
- **Success:** the brief's day 14, week 4 and 12-week goals belong to the project, not to her (persona). Yet US-24 is Must and stopping at 6 good weeks gets no ending.

## 7. Accessibility & wellbeing risks
- **The wordless heavy option still needs an accessible name.** What a screen reader announces is the real copy decision.
- **Switching keyboards between Bulgarian and English** breaks the 10-second capture. Time it with real switching.
- **Low light in the kitchen before dawn:** dark mode belongs in v1, not polish.
- **"Pages done"** needs a live-region status, and undo must not depend on a toast that disappears.
- **Mood context in US-12** puts a list of heavy days on screen; let her collapse it. The cumulative page-day count in US-15 works like a streak.
- **The designer-as-user risk** (Q5, Q6) has no mitigation beyond a feedback log. Consider freezing changes to the real copy in 7-day blocks.

## 8. Questions I'd ask the designer
1. With your irregular writing, do you want mood over time at all, or only as context for ideas?
2. Does "pick up where I left off" move your start date, your check-in day and your week-12 ending?
3. Is "what's clearer now?" a creative idea, a life insight, or either?
4. Where does v1 data live, and what happens after three weeks of not opening it in Safari?
5. Who else picks up your phone?
