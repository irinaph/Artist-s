# Phase 1 — Concept Brief v1: Artist's Sketchbook (companion for The Artist's Way)
*Approved 2026-11-15 after a critical reread. Items marked **(hypothesis)** need validation in Phase 2.*

## The book in one paragraph
*The Artist's Way* is a **12-week course** for recovering creativity. It rests on two core tools:
- **Morning pages:** three longhand pages of stream-of-consciousness writing, every morning.
- **The artist date:** a weekly block of time spent alone doing something that feeds your creative self.

Each week has a theme (Safety, Identity, Power, Integrity, Possibility, Abundance, Connection, Strength, Compassion, Self-Protection, Autonomy, Faith), a set of tasks to choose from, and a short **weekly check-in** about how the week went.

## The problem
1. **Existing apps digitize the wrong part.** Third-party apps turn morning pages into a typing journal with streaks. The book asks for **longhand** pages, and it's the **course** (weeks, dates, tasks, check-ins) that has no home. *(To confirm in competitor analysis.)*
2. **Daily practices die on broken streaks.** The research on habit apps applies directly: a reset after one missed morning feels like failure, and people quit (`research/user-complaints.md`).
3. **It's easy to lose your place.** Twelve weeks of themes, tasks and check-ins live in a book and a notebook, so it's hard to see what week you're in and what you've already done. **(hypothesis: the key assumption)**

> **Key assumption to test first in Phase 2:** *why an app, if the real work happens on paper?* Check against my own past attempts at the course: where did I stall, and what did paper fail to do?

## The idea
**A quiet companion for the 12-week course: your pages stay on paper; the app holds the path.**

You do the real work on paper and out in the world. The app tracks that you did it, shows where you are on the 12-week path, and gives every week's check-in a home. Missing a morning is normal; the progress you've made never disappears.

## Book principles → features
| Principle (book) | Feature |
|---|---|
| **Morning pages**, longhand, every day | One-tap **"Pages done"** for today. No typing the pages in the app. An optional one-line note appears only *after* the tap |
| Pages are private and not for rereading early on | The app never asks what you wrote |
| **Artist date**, weekly | This week's date: **plan it** (an optional idea) → **mark it done** |
| **12 weeks, each with a theme** | A **12-week path** showing where you are and which weeks are complete |
| **Weekly tasks** | You record which tasks you chose and did, **in your own words or from our own suggestions** (see the copyright constraint) |
| **Weekly check-in** | Day 7 of your week: pages count and artist date are **prefilled** from your taps (editable), so you only add a short reflection |
| Self-compassion and gentleness | Calm tone; no streak to break; neutral copy after a missed day |

## Core loop
```
Morning: write pages on paper → tap "Pages done" (under 5 s)
          ↓
Week: plan & take the artist date · do chosen tasks
          ↓
Day 7: weekly check-in (invited, never required) → the path moves on with the calendar → repeat ×12
          ↓
Week 12 done: course complete moment
```

## What makes it different (vs real alternatives, to be confirmed in competitor analysis)
| Alternative | What it does | Gap we fill |
|---|---|---|
| Morning-pages apps (*Morning Pages*, *AM Pages*) | Type your pages, streaks | Paper-first; covers the whole course, not just pages; no streak resets |
| The book + a notebook | Everything, but scattered | One place to see your week, path and check-ins |
| Notion / printable trackers | Static checklists | Built for the course's weekly rhythm; one-tap on a phone |
| Publisher's *Artist's Way Toolkit* app (2012) | Exercises, meditations | Apparently no longer maintained *(to verify)* |

## MVP scope (approved)
**In v1**
- Start the course: pick a start date (week 1 begins)
- **Today:** one-tap "Pages done"; an optional one-line note appears only after the tap
- **This week:** the week number and theme · the artist date (plan / done) · the tasks I chose and completed
- **Weekly check-in** on day 7: pages count and artist date prefilled (editable) + a short reflection. Invited, never required; weeks never lock
- **12-week path:** current week, completed weeks, pages and dates collected. Never resets.
- **Comeback moment** after missed days; after a **missed week**, the user chooses to **pause or continue**, with inspiration
- **Course complete** moment after week 12
- Data saved between visits

**v1.1 (first after the MVP)**
- **"Share your week" card:** a Strava-style milestone card for social media. Opt-in, no private content. See `ideas.md`

**Later** (details in `ideas.md`)
- Community; closer to the book: a small private "creative cluster"
- Reminders / notifications
- Typed pages (the book's way is longhand)
- Rereading prompts after the course
- Repeating the course a second time

## Constraints
- **Copyright:** the app must **not reproduce** the book's task lists, check-in wording or quotes. It references weeks by number and theme; tasks are typed in the user's own words or picked from **our own** suggestions.
- **My data stays mine:** before sharing the link with testers, decide where data lives; testers get a separate demo copy so they can't see or overwrite my entries.
- **Trademark:** don't use "The Artist's Way" in the app's name.
- **One-tap pages check-in in under 5 seconds** is the #1 build constraint.

## Success criteria (personal use + portfolio)
- I complete all **12 weeks** using the app
- The pages check-in takes **under 5 s**; the weekly check-in **under 2 min**
- **Accessibility:** AA contrast; status never shown by color alone; animations respect reduced motion; touch targets at least 44 px
- Every design decision traces back to the book, research, or my own use (portfolio rationale)

## Phase 1 decisions (2026-11-15)
- **Audience:** **MVP just for me.** Opening it to a small group of core users is parked in `ideas.md`.
- **MVP scope:** approved ("In v1" above)
- **Working name:** **Artist's Sketchbook** (check before launch that it isn't too close to the book's title)
- **Missed week:** the app lets the user decide: **pause the path** or **continue**, with some inspiration (our own words, no book quotes). Shown the next time they open the app.
- **Tasks:** typed in the user's own words **or** picked from suggestions (our own creative prompts, never the book's lists)
- **Start day:** the user's own start date
