# Competitor Analysis: What Already Exists for Doing The Artist's Way
**Phase 2: Discovery · desk research · 2026-11-21** (app details verified from the live App Store pages and morningpages.app FAQ the same day)
**Questions** (from `checklist.md` and the brief's "What makes it different" table):
1. What is each alternative's core loop?
2. Paper or typing: where do the pages live?
3. Does anything show patterns over time, and how?
4. What's missing for someone doing the 12-week course?

**Method:** web search, then reading the US App Store listings of the 5 morning-pages apps, the morningpages.app FAQ and the literati.tools product page. 750 Words blocks automated visits (403), so its details come from search summaries only. Templates, scan apps and Daylio also come from search summaries. No hands-on use yet: that's the Mobbin walkthrough later in Phase 2.

## How strong is the evidence?
| Tier | What it is | Trust |
|---|---|---|
| **B. User reviews** | App Store reviews (few per app), Goodreads | Medium: real voices, small numbers, some dated |
| **C. Vendor copy** | App Store listings, FAQs, product pages, template listings | High for "what exists", low for "does it work" |

**Gaps:** most apps have under 10 ratings, so review evidence is thin; prices are US-only; no Android check; 750 Words, scan apps and Daylio not verified first-hand. **Treat this as a map of the field, not a teardown.**

---

## The field at a glance
| Alternative | Where pages live | Core loop | Patterns? | Course frame | Missed day |
|---|---|---|---|---|---|
| **Morning Pages – Daily Journal** (Anastasiya Gorban; morningpages.app) · iOS/Mac/web · **4.7★, 479 ratings** · updated Nov 2026 · free; Pro $7.99/mo or $39.99/yr | **Typed**; handwriting scan (Pro) | Write → word goal → streak, badges, monthly challenges | Pro: **OpenAI reads every entry** → 10 emotions, mood (positive / negative / neutral, colored green / red / grey), topics; by day/week/month; needs 500+ words | None | **Streak with "repair days"**: 1 earned per 5 days written, auto-used on a miss (max 14) |
| **Morning pages – The Artist's Way** (Dahl & Sjöö; literati.tools) · iOS/Mac · 4.2★, 5 ratings · updated Oct 2026 · free + Premium (monthly/yearly/lifetime) | **Typed**; handwriting recognition (Premium) | Write → word goal → streak; prompts appear when you pause | **AI topic tags** per entry (on-device Apple Intelligence; Premium cloud AI sends text to literati.tools); insight charts | **Artist Dates** (plan, AI suggestions, reminders, log past ones) + **Weekly Walks**. No 12 weeks, themes or check-in | Streaks; **Vanishing Pages** deletes text after 1/7/30 days but keeps streaks |
| **AM Pages** (Mark Szymczyk) · iOS · free · 3.5★, 6 ratings · **last update 2021** | Typed | Fresh page daily, counts to ~750 words | None | None | None |
| **Pagi** (Lucas Fischer) · iOS/Mac · free + IAP · 4.5★, 10 ratings · updated Jul 2025 | Typed | Focus mode, word counter, progress bar; offline, **no tracking** | None | None | None |
| **Morning Pages: Diary & Journal** (Health & Wellness Apps Ltd) · iPhone · 2 ratings | Typed | Text field, calendar, "word grids" for goals | Light | None | — |
| **750 Words** · web *(unverified: site blocks bots)* | Typed | Write 750 words → points, badges | Per-entry stats incl. an inferred emotion | None | Streaks + "protect your streak" |
| **Scan-a-paper-page journals** (Reflect, Journal Scanner, Journal Mate) *(search summaries)* | **Paper**, photographed | Photo → OCR → auto date + mood tags → ask AI | **AI reads the full page** | None | — |
| **Daylio** *(search summaries)* | No writing | Two taps: mood + activities | Charts, mood–activity links (deeper stats paid) | None | Streaks |
| **Notion templates & printables** ($0–$5) | Paper or typed | Tick boxes: pages, artist date, check-in, tasks | None (static) | **Yes**: 12 weeks, artist dates, check-ins | Nothing happens |
| **Hobby web apps** (2 open-source PWAs on GitHub) | **Paper notebook** + phone | Artist-date toggle, note field; data only on the phone | None | Partly | — |
| **My Artist's Way Toolkit & App** (Tarcher/Penguin, 2012) | Web notebook | Daily inspirations, notebook, artist dates | None known | Yes (official) | — |
| **The Morning Pages Journal** (paper, official) | **Paper** | Lined pages, instructions, quotes | None | Not by week | — |

---

## Findings

### Finding 1: Every morning-pages app is a typing app, and the two serious ones are actively growing
All five apps on the App Store have you **type** the pages. Two are dormant or minimal (AM Pages, last updated 2021; Diary & Journal, 2 ratings). Two are actively built, with updates in Oct–Nov 2026: **Morning Pages – Daily Journal** (the market leader, 479 ratings) and **Dahl & Sjöö's Morning pages**. Both have added handwriting scanning as a paid extra; typing stays the core loop. [C]

One reviewer said they switched from paper to the app because they didn't always have their notebook with them. [B]

> **What it means for us:** "paper-first" is still a real difference. The tradeoff is real too: some people *want* to leave paper. We stay paper-first because the book asks for longhand and it's how I practice; this is a deliberate choice for our user, not a gap in the market.

### Finding 2: Pattern insights come from AI reading your private pages, and the accuracy is openly shaky
- **Morning Pages – Daily Journal** sends every entry to **OpenAI** to detect emotions, mood and topics, and needs **500+ words** a day to work. Its own FAQ says insights "won't always be 100% accurate" and tells users who **feel judged** to switch them off. [C]
- A user review: "Great idea, **disappointing statistics**" (2020), about the app labelling writing positive or negative. The developer replied in Oct 2026 that insights were rebuilt. [B]
- **Dahl & Sjöö** auto-generates topic tags with on-device AI; its Premium cloud AI sends text to its own server. [C]
- Scan apps (Reflect, Journal Scanner) do the same with photos of paper pages. [C, unverified]

> **What it means for us:** "paper + patterns" alone is **not** our differentiator. What is:
> - **The app never sees the pages.** Patterns come from **my own 10-second summary** (mood, themes, one idea), not from machine-reading private writing.
> - It works on a **short morning** too: AI insights need 500+ words, our capture doesn't care how much I wrote.
> - **I name my own mood,** so there's nothing to "feel judged" by. That fits our calm tone and avoids the leader's known weak spot.
> - It matches the book's privacy ethic (pages aren't for rereading early on; `artists-way-practitioners.md` Finding 4).

### Finding 3: Privacy is something people actively look for
- Pagi's most recent review praises it as the only writing app found that **doesn't collect data**, "in these uncertain times with AI mining". [B]
- Dahl & Sjöö's **Vanishing Pages** (text deleted after 1/7/30 days, streaks kept) is praised in its top review: "frees me up to really write freely". [B]
- Its privacy label, by contrast, lists **user content and coarse location linked to identity**. [C]

> **What it means for us:** "your pages never enter the app" is a privacy promise that's simpler and stronger than vanishing text or opt-out AI. Worth making visible in onboarding copy (Phase 4).

### Finding 4: One app now covers artist dates, but nobody covers the course itself
- **Dahl & Sjöö's app has Artist Dates** (plan, AI suggestions, reminders, log past outings) and Weekly Walks. This corrects the brief's assumption that no app tracks artist dates. [C]
- **No app** has the 12-week path, weekly themes, a weekly check-in, or support for the early weeks when people quit (`artists-way-practitioners.md`).
- Notion templates and printables have the course structure but are static checkbox logs. [C]
- The only official app (2012 Toolkit) had the course and artist dates; I couldn't confirm it still exists, and its name now belongs to a **2025 book**. [C]

> **What it means for us:** the artist date is now table stakes, not a differentiator. Our difference is the **course frame + early-weeks support + gentle missed-week handling**, around a paper practice.

### Finding 5: Streak pressure is built in everywhere, even in the softened versions
- The market leader **softens** streaks with "repair days" (earned by writing 5 days in a row, used automatically on a miss), but still centres the experience on streaks, 18+ streak and word-count badges, widgets showing the streak, and month-long writing challenges. [C]
- Dahl & Sjöö keeps streak counts even when page text vanishes. 750 Words lets you "protect your streak". [C]

> **What it means for us:** confirms "no streak resets" (`user-complaints.md`). Repair days still treat a missed morning as damage to be repaired; our comeback moment and pause-or-continue choice don't count damage at all.

### Finding 6: Low-friction mood logging is proven (Daylio)
Daylio's two-tap, no-typing logging is praised as the low-friction end of the market; its deeper stats are paid. [B/C]

> **What it means for us:** supports the "under 5 s tap, then optional ~10 s capture" approach. In a quick Mobbin test, Daylio didn't come up by name, but similar mood check-ins did (e.g. 5 Minute Journal), so there are references for the capture screen in Phase 3.

### Finding 7: The paper journal is not enough even for its own users
Reviewers of the official *Morning Pages Journal* say there aren't enough pages for the whole program (one edition has 252 pages, about 84 days). It has instructions and quotes, but no week structure. [B]

> **What it means for us:** paper is the right place for the pages, but it gives no overview, the same gap as in my own attempts.

### Finding 8: Accessibility is weak across the field
None of the five App Store listings declares any accessibility features (one app's changelog mentions adding VoiceOver support). The leader's mood chart uses **green / red / grey**; whether it relies on color alone isn't visible from the listing. [C]

> **What it means for us:** our criteria (status never by color alone, a text alternative for the pattern view) are a small but real difference, and a good case-study point. Check hands-on during the Mobbin walkthrough.

---

## Updated "What makes it different"
| Alternative | What it does | Gap we fill |
|---|---|---|
| Morning-pages apps (*Morning Pages – Daily Journal*, Dahl & Sjöö's *Morning pages*, *Pagi*, *AM Pages*, 750 Words) | Type your pages; word goals; streaks and badges; paid AI insights; one has artist dates | Paper-first; **no streaks to protect**; the 12-week frame and early-weeks support |
| AI insights (OpenAI / on-device) and scan-and-AI journals | Read the full page to infer mood, emotions, topics; need 500+ words; accuracy openly imperfect | **The app never reads the pages**: I name my mood, themes and one idea myself, on any length of morning |
| Mood trackers (*Daylio*) | Fast mood + activity logs, charts | Tied to the creative practice: themes and ideas → creative direction |
| Notion templates / printables | Static 12-week checklists | One tap on a phone; patterns build up; gentle missed-day handling |
| Paper journal / notebook | The pages, no overview | Patterns over time + the course frame |
| 2012 *My Artist's Way Toolkit* | Inspirations, notebook, artist dates | Status unconfirmed; the name is now a 2025 book |

---

## Candidates for decisions (for you to accept or change)
1. **Sharpen the positioning to "your pages stay private, even from the app".** AI insights and scanning already exist; our real difference is that patterns come from my own short words, never from reading the pages. Replace the brief's differentiator table with the version above (it also corrects the artist-date assumption).
2. **No scan, OCR or AI reading of pages in the MVP, as a stated principle.** Reasons: the book's privacy ethic, the writing-for-the-tag risk, and the leader's own admission that AI insights can be wrong and feel judging. Log it so it's in the case study.
3. **Add Mobbin references for Phase 3:** mood check-ins (5 Minute Journal and similar) for the capture screen; the leader's Insights screen as a *contrast* example for the pattern view.
4. **Naming check:** two apps are already called "Morning pages", one with "The Artist's Way" as its subtitle. Our working name, Artist's Sketchbook, avoids both; keep it on the pre-launch trademark check.

---

## Sources
**App Store listings and product pages (C, B for quoted reviews)**, all read 2026-11-21
- [Morning Pages – Daily Journal (Anastasiya Gorban)](https://apps.apple.com/us/app/morning-pages-daily-journal/id1223874080) · [morningpages.app FAQ](https://morningpages.app/faq/) · [morningpages.app](https://morningpages.app/)
- [Morning pages – The Artist's Way (Dahl & Sjöö)](https://apps.apple.com/us/app/morning-pages/id6738604034) · [literati.tools product page](https://www.literati.tools/morning-pages/en) · [Dahl & Sjöö studio](https://www.dahlsjoo.com/)
- [AM Pages](https://apps.apple.com/us/app/am-pages/id1447417846)
- [Pagi – Morning Pages & Diary](https://apps.apple.com/us/app/id1586446074)
- [Morning Pages: Diary & Journal](https://apps.apple.com/us/app/id6714479684)

**Search summaries only (C)**
- 750 Words: [site](https://www.750words.com) · [FAQ](https://750words.com/faq) · [Working on V2 (pricing post)](https://medium.com/750-words/working-on-750-words-v2-321a7284153c)
- Scan-and-AI journals: [Reflect (AlternativeTo)](https://alternativeto.net/software/reflect-ai-journal-diary/about/) · [Journal Scanner (App Store)](https://apps.apple.com/us/app/-/id6695735974) · [Journal Mate (App Store)](https://apps.apple.com/app/journal-mate/id1533808328)
- Daylio: [Headway review](https://makeheadway.com/blog/daylio-review/) · [Choosing Therapy review](https://www.choosingtherapy.com/daylio-app-review/)

**Course trackers (C)**
- [The Artist's Way Companion (Notion template gallery)](https://www.notion.com/templates/the-artist-s-way-companion)
- [Hurley Winkler: 12-week printable tracker](https://hurleywinkler.gumroad.com/l/artists-way-tracker?layout=profile) · [Etsy printable toolkit](https://www.etsy.com/listing/4301253561/the-artists-way-toolkit-printable)
- Hobby web apps: [artist-way-companion](https://github.com/abasarcadi-ops/artist-way-companion) · [artist-way-compation](https://github.com/abasarcadi-ops/artist-way-compation)

**Official products (C, B)**
- 2012 app: [Adweek](https://www.adweek.com/performance-marketing/penguin-launches-artists-way-toolkit-app/) · [Shelf Awareness](https://www.shelf-awareness.com/theshelf/2012-02-02/app_of_the_day:_my_artist_s_way_toolkit_app.html) · [Publishers Lunch](https://lunch.publishersmarketplace.com/2012/01/enews-penguin-launches-mobile-platform-self-publishing-capabilities-from-nelson-literary-agency/) · [Big Girl Blue review (2012)](https://biggirlblue.com/2012/03/10/the-artist-way-toolkit-app-review/)
- 2025 book with the same name: [Macmillan](https://us.macmillan.com/books/9781250344977/theartistswaytoolkit/)
- Morning Pages Journal: [Julia Cameron Live](https://juliacameronlive.com/book/the-artists-way-morning-pages-journal) · [NetGalley](https://netgalley.com/catalog/book/99993) · [Walmart (page count)](https://www.walmart.com/ip/250821)
