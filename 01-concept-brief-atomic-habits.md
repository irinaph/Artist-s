# Phase 1 — Concept Brief

## The problem
Most habit apps treat a habit as a checkbox and motivation as a streak counter. That has three failure modes:

1. **Goal-first, not identity-first.** "Read 20 pages" is a task. Nothing connects it to *why*, so motivation fades once novelty wears off.
2. **Streaks punish the inevitable.** One missed day resets the counter to zero, which feels like losing everything. That's often the moment people quit the app entirely.
3. **No help with the hard part.** Apps track whether you did the habit, but don't help design the habit so it's easy to do in the first place.

## The idea
**A habit app where every check-in is a vote for the person you're becoming.**

You start with an identity, not a goal. You design each habit using the Four Laws of Behavior Change, so it's built to stick before day one. Missing a day is normal; the only rule is *never miss twice*.

**One-liner:** *Small habits, cast as votes for who you want to be.*

## Book principles → features

| Principle (Atomic Habits) | Feature |
|---|---|
| **Identity-based habits:** lasting change comes from who you believe you are | Onboarding starts with "Who do you want to become?" Each habit is linked to an identity |
| **Every action is a vote** for an identity | Check-ins are counted as **votes**, shown per identity ("47 votes for *I am a reader*") |
| **Law 1: Make it obvious:** implementation intentions and habit stacking | Habit builder asks for a **cue**: "After I [current habit], I will [new habit]" or "At [time] in [place]" |
| **Law 2: Make it attractive:** temptation bundling | Optional **pairing** field: "I'll only [thing I enjoy] while/after doing this" |
| **Law 3: Make it easy:** the Two-Minute Rule | Every habit has a **2-minute version**. Doing the 2-minute version counts as a full vote |
| **Law 4: Make it satisfying:** immediate reward, habit tracking | Satisfying one-tap check-in with micro-animation. Optional reward note |
| **Never miss twice** | No streak reset. One miss = neutral, with no-blame copy. The day after a miss shows a **comeback moment**. Nudge only when a second miss is about to happen |
| **Getting 1% better** compounds | Progress view shows a gentle compounding curve over time, not a fragile streak number |
| **Plateau of latent potential:** results lag behind effort | Early-days messaging that reframes slow visible progress ("valley of disappointment"), with real numbers: habits take **~66 days on average (18–254)**, not 21 |

## Core loop
```
Choose identity → Design habit (4 Laws) → Cue happens → Do 2-min version
      ↑                                                        ↓
 Weekly reflection  ←  Votes add up per identity  ←  One-tap check-in
```

## What makes it different
| Typical habit app | This app |
|---|---|
| Streak counter, resets to 0 | Vote count, never resets; "never miss twice" rule |
| "Add habit" = name + frequency | Habit builder walks through the 4 Laws |
| Goal / task framing | Identity framing |
| Success = full completion | Success = showing up (2-minute version counts) |

## MVP scope
**In v1**
- Onboarding: choose 1–3 identities
- **Start with 1–3 habits** (more can be added once those stick)
- Habit builder (cue/stack, pairing, 2-minute version, schedule)
- **Flexible frequency:** daily or "X times per week"
- Today view with one-tap check-in (full or 2-minute version)
- Never-miss-twice status and nudge, plus a **comeback moment** the day after a miss
- Progress: votes per identity, history calendar
- Weekly reflection (2–3 quick prompts)
- Data saved between visits

**Later**
- Breaking bad habits (inverted laws, habit scorecard)
- Habit contracts / accountability partner
- Push notifications (limited on web)
- Habit templates library

## Research-driven updates (2026-11-15)
Based on `research/user-complaints.md`:
- The core bets are validated: never miss twice, votes that never reset, habit-stacking cues (cues beat reminders), the 2-minute version.
- **One-tap check-in in under 5 seconds** is the #1 build constraint (logging fatigue is a top reason for quitting).
- Added: the 1–3 habit start limit, flexible frequency, the comeback moment.
- **Open design questions for Phase 3:**
  - What does "never miss twice" mean for a 3-times-a-week habit?
  - How do people remember to open the app without relying on reminders?

## Success criteria (personal use + portfolio)
- I use it daily for 30 days without it feeling like a chore
- Creating a habit takes under 2 minutes
- Checking in takes under 5 seconds
- Each design decision traces back to a book principle or user need (portfolio rationale)

## Phase 1 decisions (2026-11-15)
- **Name:** **Grains**
- **Identity input:** short, editable suggestions plus a free-text option
- **Tone:** calm and reflective, like a journal. No points or badges; the satisfying moment is the check-in itself (micro-animation).
