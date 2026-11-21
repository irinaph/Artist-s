# Concept Brief v2: Artist's Sketchbook (companion for The Artist's Way)
*v2, 2026-11-15: re-centered after my self-interview (`research/my-past-attempts.md`). v1 (in `archive/`) made "the 12-week path" the core; the interview showed my real need is seeing my own patterns.*

## The book in one paragraph
*The Artist's Way* is a **12-week course** for recovering creativity. It rests on two core tools:
- **Morning pages:** three longhand pages of stream-of-consciousness writing, every morning.
- **The artist date:** a weekly block of time spent alone doing something that feeds your creative self.

Each week has a theme (Safety, Identity, Power, Integrity, Possibility, Abundance, Connection, Strength, Compassion, Self-Protection, Autonomy, Faith) and ends with a short weekly check-in.

## The problem (from my two past attempts)
1. **Paper can't show me my patterns.** The pages were a way to get to know myself again, but a notebook gives no overview of my **themes, moods and ideas** over time, and no direction for creative plans.
2. **The first weeks are the danger zone.** Both my attempts ended in the first two weeks (day ~10 and day 3); other practitioners mostly stall in weeks 2–5 (`research/artists-way-practitioners.md`). It wasn't from losing track, but from:
   - **Permission:** feeling "too old, with too many responsibilities" for creative play
   - **Time:** responsibilities crowded out the artist date, even with a specific wish (an exhibition)
   - **Emotional weight:** the pages surfaced anger, and nothing helped me regroup constructively
3. **Daily practices die on broken streaks.** A reset after a missed morning feels like failure (`research/user-complaints.md`).

## The idea
**Your pages stay on paper; the app reflects your patterns back to you.**

You write by hand, as the book asks. Afterwards, the app takes about ten seconds to capture something *about* the entry: a mood, a theme or two, one idea. It never records the entry itself. Over the weeks, those small captures build a picture of who you're becoming and where your creative energy wants to go. The app is especially gentle in the first four weeks, when people are most likely to stop.

## Book principles → features
| Principle (book) / need (me) | Feature |
|---|---|
| **Morning pages**, longhand, every day | One-tap **"Pages done"** (under 5 s). No typing the pages in the app. A shorter morning counts too (quiet option) |
| Pages are private; not for rereading early on | The app never asks what you wrote. You choose what to capture *about* it, in your own words |
| **Getting to know myself again** (me) | Optional **10-second capture** after the tap: **mood**, **1–2 themes**, **one idea** |
| **Direction for creative plans** (me) | A **pattern view**: moods over time, recurring themes, collected ideas. Low-key in weeks 1–2 (empty state, no pushed insights) |
| **Artist date**, weekly | Plan it (an optional idea) → mark it done. **A small date counts** (e.g. 30 minutes) |
| **Seeing what the practice produces** (me) | When an artist date is done: an optional **"what came out of it?"** note (one sentence), shown in the pattern view next to my ideas |
| Permission to create (me: "too old, too busy") | Gentle framing in our own words, strongest in weeks 1–4 and tapering off |
| Hard days (me: anger, couldn't regroup) | When I log a heavy mood, a calm, optional prompt to note one constructive next step |
| **12 weeks, each with a theme** | A **light path frame**: which week I'm in and its theme. Not the main screen |
| **Weekly check-in** | Day 7: pages count and artist date prefilled (editable) + a short reflection. Invited, never required |
| Self-compassion and gentleness | Calm tone; no streak to break; weeks never lock |

## Core loop
```
Morning: write pages on paper → tap "Pages done" (under 5 s)
          → optional 10 s capture: mood · themes · one idea
          ↓
Week: plan & take a (small) artist date → optional "what came out of it?" note
          ↓
Day 7: weekly check-in (invited) → the path moves on with the calendar
          ↓
Over time: the pattern view shows my moods, themes, ideas and what came out of my dates → direction for creative plans
          ↓
Week 12: course complete moment
```

## What makes it different (confirmed in `research/competitors.md`, 2026-11-21)
**Positioning: your pages stay yours. Nothing is read unless you choose.** In v1, patterns come only from my own short notes; any future reading of pages is opt-in (`ideas.md`).

| Alternative | What it does | Gap we fill |
|---|---|---|
| Morning-pages apps (*Morning Pages – Daily Journal*, Dahl & Sjöö's *Morning pages*, *Pagi*, *AM Pages*, 750 Words) | Type your pages; word goals; streaks and badges; paid AI insights; one has artist dates | Paper-first; **no streaks to protect**; the 12-week frame and early-weeks support |
| AI insights and scan-and-AI journals | Read the full page to infer mood, emotions, topics; need 500+ words; accuracy openly imperfect | **Nothing is read unless I choose**: I name my mood, themes and one idea myself, on any length of morning |
| Mood trackers (*Daylio*) | Fast mood + activity logs, charts | Tied to the creative practice: themes, ideas and what my dates produce → creative direction |
| Notion templates / printables | Static 12-week checklists | One tap on a phone; patterns build up; gentle missed-day handling |
| Paper journal / notebook | The pages, no overview | Patterns over time + the course frame |
| 2012 *My Artist's Way Toolkit* | Inspirations, notebook, artist dates | Status unconfirmed; the name is now a 2025 book |

## MVP scope (approved, re-centered 2026-11-15)
**In v1**
- Start the course: pick a start date (week 1 begins)
- **Today:** one-tap "Pages done" (a shorter morning counts too) → optional 10 s capture (mood, 1–2 themes, one idea)
- **Pattern view:** moods over time, recurring themes, collected ideas; low-key in weeks 1–2
- **Artist date:** plan (an optional idea) / done; small dates count; optional "what came out of it?" note (text only, no photos in v1)
- **Early support, weeks 1–4 (tapering):** permission framing; a calm "one constructive next step" prompt on heavy days, saying an early dip is normal
- **Weekly check-in** on day 7: prefilled + a short reflection. Invited, never required; weeks never lock
- **Light 12-week path:** current week and theme
- **Comeback moment** after missed days; after a **missed week**, I choose **pause or continue**, with inspiration
- **Course complete** moment after week 12
- Data saved between visits

**v1.1 (first after the MVP)**
- **"Share your week" card:** a Strava-style milestone card. Opt-in, no private content. See `ideas.md`

**Later** (details in `ideas.md`)
- Recording weekly tasks (parked in v2: my attempts never got that far; the capture takes its place)
- Community; closer to the book: a small private "creative cluster"
- Opening the app to core users
- **AI handwriting scan** for richer analysis: opt-in, after week 8 (conditions in `ideas.md`)
- Photos for the artist-date note
- Reminders / notifications · typed pages · rereading prompts after the course · repeating the course

## Constraints
- **Copyright:** never reproduce the book's task lists, check-in wording or quotes. Weeks are referenced by number and theme; suggestions and inspirations are our own content.
- **Trademark:** don't use "The Artist's Way" in the app's name.
- **One-tap pages check-in in under 5 seconds** is the #1 build constraint; the capture is always optional and comes after it.
- **Not a mental-health tool:** calm, acknowledging copy is in scope; therapy-like features are not.
- **My data stays mine:** before sharing with testers, decide where data lives; testers get a separate demo copy.

## Success criteria (personal use + portfolio)
- I get **past day 14** and **week 4**, then complete all **12 weeks**
- After 2 weeks, the pattern view shows me **at least one pattern I didn't notice** on paper
- The pages check-in takes **under 5 s**; the capture **about 10 s**; the weekly check-in **under 2 min**
- **Accessibility:** AA contrast; status never shown by color alone; the pattern view has a text alternative and isn't color-only; animations respect reduced motion; touch targets at least 44 px
- Every design decision traces back to the book, research, or my own use (portfolio rationale)

## Decisions so far
- **Audience:** MVP just for me; opening it to core users is parked in `ideas.md`
- **Working name:** **Artist's Sketchbook** (check before launch that it isn't too close to the book's title)
- **Missed week:** I decide: pause the path or continue, with inspiration (our own words). Shown the next time I open the app
- **Start day:** my own start date; the weekly check-in falls on day 7
- **Tasks:** ~~own words or suggestions~~ → parked in v2 (`ideas.md`)
- **Re-centered (v2):** from "the app holds the path" to "the app reflects my patterns back to me"
- **Creative output (2026-11-21):** the artist date gets an optional "what came out of it?" note; the AI handwriting scan is parked for later
