# Artist's Sketchbook — Project Plan
*(working name; companion app for The Artist's Way)*

## Decisions
- **Audience (2026-11-15):** **MVP just for me**, also documented as a portfolio case study. Briefly considered opening it to a small group of core users; kept single-user to keep the MVP small. Opening to others is parked in `ideas.md`.
- **Platform:** Mobile-first web, delivered as a working link (Claude artifact with a built-in database)
- **Claude's role (2026-10-31):** project manager by default, user persona only on request (CLAUDE.md). Keeps scope and decisions on track while I own the design calls.
- **Reconcept (2026-11-15):** dropped the Atomic Habits concept. The official app, Atoms, already offers identity-based habits and a Four Laws habit builder, so two of our four differentiators weren't different.
- **Book: The Artist's Way by Julia Cameron (2026-11-15):** no current official app (only a dated 2012 publisher toolkit and third-party morning-pages apps built on streaks); progress is built into the book as a 12-week course; I've read it and want to practice it, so I'm the primary user.
- **MVP focus (2026-11-15, updated in v2):** a companion for the course whose core value is reflecting my patterns back to me (see brief v2).
- **Tone: calm & reflective (2026-11-15, carried over):** research shows game layers overwhelm and guilt makes people quit; also fits the book's gentle, self-compassionate voice.
- **No streak resets + comeback moment (2026-11-15, carried over):** research on broken streaks applies to any daily practice (research/user-complaints.md).
- **Solve "remembering to open the app" in Phase 3 (2026-11-15, carried over):** reminders don't build habits, but users who stop opening the app quit.
- **Community parked; share card is v1.1 (2026-11-15):** a community needs many users, accounts and moderation (bigger than the MVP) and the pages are private. A Strava-style "share your week" card solves accountability, celebration and inspiring others with no private content; it comes after real use shows whether I'd share. Details in `ideas.md`.
- **MVP scope approved (2026-11-15):** the "In v1" list in `01-concept-brief.md`; small enough to ship fast, then expand from `ideas.md` based on my own use.
- **Name: Artist's Sketchbook (working, 2026-11-15):** the sketchbook fits the paper-first idea. Check before launch that "Artist's" isn't too close to the book's trademarked title.
- **Missed week: the user decides (2026-11-15):** the app asks whether to pause the path or continue, and offers inspiration (our own content, never book quotes). Gives control instead of punishment; shown when the user next opens the app.
- **Tasks: own words or suggestions (2026-11-15):** typing keeps it personal; suggestions speed it up. Suggestions are our own creative prompts, never the book's task lists (copyright).
- **Start day: the user's start date (2026-11-15):** week 1 begins whenever they start, so there's no waiting for a fixed weekday.
- **Critical reread of the brief (2026-11-15), all recommendations accepted:**
  - Check-in on **day 7** of my week, not Sunday: follows from starting on my own date.
  - **Weeks never lock;** the check-in is invited, not required: a gate would punish, against the calm tone.
  - Check-in **prefills** pages and artist date from my taps: asking twice is logging fatigue.
  - **Course complete** moment added to the MVP: the course needs an ending (and later, the share card's best content).
  - **Testers get a demo copy:** a shared link must not expose or overwrite my data.
  - The optional note appears **only after** the pages tap: keeps the tap under 5 s.
  - "Why an app if the work is on paper?" is the **first thing Phase 2 tests**.
- **Re-centered the concept, brief v2 (2026-11-15):** my self-interview showed the key assumption ("it's easy to lose your place") didn't hold: I never got past week 2, and a dated notebook was enough. What paper failed at was showing me my **themes, moods and ideas** over time. The app now **reflects my patterns back to me**: one-tap "Pages done" → optional 10 s capture → a pattern view; extra support in days 1–14 (permission, small artist dates, heavy days); the 12-week path becomes a light frame. v1 is archived. (`research/my-past-attempts.md`)
- **Weekly tasks parked (2026-11-15):** my attempts never got that far, and the capture replaces it as the second core feature, keeping the MVP small.
- **Early support covers weeks 1–4, tapering (2026-11-21):** practitioner accounts place most stalls in weeks 2–5, not only days 1–14; same features, longer window, easing off so it doesn't feel patronizing. (`research/artists-way-practitioners.md`)
- **A shorter morning counts as "Pages done" (2026-11-21):** people who finished often shrank the pages; a quiet option with neutral wording, never the default ask, so the book's three pages stay the norm.
- **Pattern view low-key in weeks 1–2 (2026-11-21):** visible from day 1, with an empty state until captures build up and no pushed insights; keeps writing and reviewing apart, echoing the book's wait-before-rereading advice.
- **Heavy-day copy says an early dip is normal (2026-11-21):** expressive-writing research shows a short-term rise in distress before benefits; our own words, written in Phase 4.
- **Competitor analysis, the field (2026-11-21):** every morning-pages app is typed-first; their pattern insights come from AI reading the pages (OpenAI, 500+ words, accuracy openly imperfect); one app now has artist dates, but none has the 12-week course or early-weeks support. (`research/competitors.md`)
- **Artist-date "what came out of it?" note in the MVP (2026-11-21):** marking an artist date done offers an optional one-sentence note that feeds the pattern view, so I see my ideas next to what I acted on; it directly serves "direction for creative plans". No photos in v1 (storage, extra build).
- **The 10-second note is how v1 builds patterns (2026-11-21):** works on a short morning, nothing to feel judged by, and the app never sees the pages in v1.
- **AI handwriting scan parked for later (2026-11-21):** I want richer analysis long term; parked because it's a big build, it overlaps the market leader, and reading the pages needs care with the book's no-rereading period. Conditions in `ideas.md`.
- **Positioning: "your pages stay yours: nothing is read unless you choose" (2026-11-21):** AI reading and scanning already exist, so paper + patterns alone isn't different; patterns from my own notes, with any future reading opt-in, is. Brief's differentiator table replaced.
- **Mobbin references for Phase 3 (2026-11-21):** mood check-ins (e.g. 5 Minute Journal) for the capture screen; the market leader's Insights screen as a contrast example for the pattern view.
- **Name stays Artist's Sketchbook (2026-11-21):** two apps are already called "Morning pages" (one subtitled "The Artist's Way"); ours avoids both. Trademark check before launch still stands.
- **Not a mental-health tool (2026-11-15):** the pages can surface heavy feelings; the app responds with calm copy and an optional ~~"one constructive next step"~~ "what's clearer now?" (changed 2026-11-21), never therapy-like features.

- **Persona design candidates decided (2026-11-21):** (`research/persona.md`)
  - **Log late: today + yesterday:** I open the app whenever I remember; older days go through the comeback flow so logging never becomes catch-up homework.
  - **The mood asks how the pages felt:** still clear a day later, and it records what the patterns are for, not my afternoon.
  - **Remembering: paper cue + home-screen shortcut; reminders stay parked:** the notebook is my only constant, and routine cues beat reminders (a web app has no reliable push).
  - **Theme and idea are two free-text fields, no medium tag:** themes = what the pages were about, ideas = creative ideas; a medium picker would cost a tap in a 10 s capture.
  - **Heavy day → room first, then "what's clearer now?" (replaces "one constructive next step"):** my ideas flowed once I'd unloaded; "next step" read like a to-do.
  - **On a heavy day the app never cheers me up; help resources appear only if I turn them on:** upbeat copy dismisses the feeling, and unasked resources would make it a mental-health tool.
  - **Weekly patterns in the day-7 check-in; the "new pattern" card is parked:** with irregular writing and no real data yet, rules would fire on noise and feed the "patterns say nothing new" quit risk.
  - **Bilingual notes with manual theme merge; Cyrillic-ready fonts:** "работа" and "work" would otherwise split the very patterns the app exists to show.
  - **UI in English only for v1:** one set of copy keeps tone work manageable and suits the portfolio; Bulgarian UI parked.
  - **Irregular writing is normal; comeback is a core flow:** I write when I need to, so a gap is the expected case, never a failure.
  - **Success = real insight, not completion:** 6 weeks with real insight counts; 12 weeks is the stretch goal.

- **Journey candidates decided (2026-11-27):** (`research/journey.md`, after the persona role-play)
  - **An always-available "so far" recap of progress, moods and ideas:** insight counts as success whenever I stop, and moods are the context for my ideas; built as a mode of the pattern view, not a separate screen. 
  - **One tap turns a captured idea into the next artist date plan:** closes the loop from idea to action (goal 2), using text I already wrote.
  - **The pattern view leads with recurring ideas; moods and themes are context:** in the role-play, ideas were what made the check-in worth it and what would save thin patterns.
  - **"Start again from week 1" stays, as a secondary option:** some may want it, but starting over is the fear, so the primary choices are pick up / join the current week, and "pause" gets renamed.
  - **Role-play details confirmed:** I write in the kitchen before everyone wakes; I have kids. Added to the persona as [me].
- **User stories, export (2026-11-27):** keep export in v1 (Must) as a single "Download my notes" file, export only; import is parked for v1.1. Twelve weeks of patterns in one artifact is a single point of failure, and export is what makes "never lost / never locked in" true.
- **User stories, cut order (2026-11-27):** if the build runs long, cut the Should stories US-21 (help resources) → US-15 ("so far" recap) → US-18 (idea → artist date). US-21 is invisible by default; US-18 is the only one that turns a pattern into action, so it stays longest.

### Superseded by the reconcept (kept for the case study)
- ~~MVP focus: building good habits~~ · ~~Start with 1–3 habits~~ · ~~Flexible frequency~~ · ~~Identity input: suggestions + free text~~ · ~~Name: Grains~~. These were Atomic Habits-specific. The old brief is in `archive/01-concept-brief-atomic-habits.md`.

## Phases
| # | Phase | Deliverable |
|---|---|---|
| 1 | Concept: book principles → features, sharpen differentiator | Concept brief |
| 2 | Users & MVP scope | Persona + MVP feature list |
| 3 | UX flows: start, pages tap + capture, pattern view, artist date, weekly check-in, days 1–14 support; Mobbin references | Flow maps + reference board |
| 4 | UI direction | Style guide + key screens |
| 5 | Build: mobile-first web app as a Claude artifact | Working link |
| 6 | Test & iterate: use it through the 12 weeks | v1.1 |

## Portfolio notes
Document decisions and rationale at each phase so the process can be turned into a case study.
**Pivot story:** research + a critical review showed the first concept was too close to the official Atomic Habits app → reconcept around a book with no official companion app.
