# Competitor Analysis: What Already Exists for Doing The Artist's Way
**Phase 2: Discovery · desk research · 2026-11-21**
**Questions** (from `checklist.md` and the brief's "What makes it different" table):
1. What is each alternative's core loop?
2. Paper or typing: where do the pages live?
3. Does anything show patterns over time, and how?
4. What's missing for someone doing the 12-week course?

**Method:** web search only. App Store pages, vendor sites and 750 Words could not be opened from this session (network blocked), so app details come from search-result summaries of those pages. **Prices, ratings and features can be out of date or differ by country; verify in the store before quoting them in the case study.** No hands-on testing yet: that's the Mobbin walkthrough later in Phase 2.

## How strong is the evidence?
| Tier | What it is | Trust |
|---|---|---|
| **B. User reviews** | App Store reviews quoted in search summaries; Goodreads reviews | Medium: real voices, few of them, some dated |
| **C. Vendor copy** | App Store listings, FAQs, template and printable listings | Good for "what exists", low for "does it work" |

**Gaps:** no ratings counts or review volumes; no Android check; no hands-on use. **Treat this as a map of the field, not a teardown.**

---

## The field at a glance
| Alternative | Where pages live | Core loop | Patterns? | Course frame (12 weeks, artist dates) | Missed day |
|---|---|---|---|---|---|
| **Morning Pages** (Dahl & Sjöö), iOS/Mac/web | **Typed** in the app; **handwriting scan** added | Write 3 pages → word count → stats | **AI** reads entries (via OpenAI) → emotions, topics, mood by day/week/month (Premium) | None found | Streaks + badges |
| **Morning Pages – Daily Journal** (Gorban) | Typed | Write → AI "emotional insights" | AI insights, mood tracking (subscription) | None | Reminders; streak behavior unclear |
| **Morning Pages: Diary & Journal** | Typed | Text field + calendar + "word grids" for key words/goals | Light (calendar, key words) | None | Unclear |
| **AM Pages** (Szymczyk), iOS, free | Typed | Fresh page daily, word counter to ~750 words | None | None | None found |
| **Pagi**, iOS, one-time ~$12 | Typed | Write → word counter + progress bar; offline, no tracking | None | None | None found |
| **750 Words**, web, ~$5/mo (dated figure) | Typed | Write 750 words → points, badges, animal icons | Per-entry stats incl. an inferred **emotion**, metadata links across entries | None | **Streaks**; a paid-style "protect your streak" patch for one missed day |
| **Scan-a-paper-page journals** (Reflect, Journal Scanner, Journal Mate) | **Paper**, photographed | Photo → OCR → auto date + **mood tags** → ask AI about past entries | **AI reads the full page text** | None | — |
| **Daylio** (mood tracker) | No writing needed | Two taps: mood + activities | Charts, mood–activity links (deeper stats paid) | None | Streaks |
| **Notion templates & printables** ($0–$5, Gumroad/Etsy/Notion gallery) | Paper or typed | Tick boxes: pages, artist date, weekly check-in, tasks | None (static) | **Yes**: 12 weeks, artist dates, check-ins | Nothing happens |
| **Hobby web apps** (2 open-source PWAs on GitHub) | **Paper notebook** + phone | Toggle artist date, note field; data only on the phone | None | Partly (weeks, artist date) | — |
| **My Artist's Way Toolkit & App** (Tarcher/Penguin, 2012) | Web notebook (typed) | Daily inspirations, interactive notebook, record artist dates | None known | Yes (official) | — |
| **The Morning Pages Journal** (paper, official) | **Paper** | Lined pages, instructions, quotes | None | Not structured by week | — |

---

## Findings

### Finding 1: The morning-pages apps are typing apps
Every dedicated morning-pages app found (Morning Pages, AM Pages, Pagi, Diary & Journal, 750 Words) has you **type** the pages. Their loop is write → word count → streak/stats. That goes against the book's longhand rule, and against my own practice (`my-past-attempts.md`). [C]

> **What it means for us:** "paper-first" is still a real difference from the morning-pages category, as the brief assumed.

### Finding 2: The closest competitors are scan-and-AI journals, and they read your private pages
This wasn't in the brief. A newer group of apps **is** paper-first and **does** show patterns:
- **Reflect** photographs a paper page, runs OCR, dates it and **tags mood automatically**, and lets you ask an AI about past entries. [C]
- **Journal Scanner** does the same with AI pattern and emotion insights. [C]
- The leading **Morning Pages** app added a **handwriting scan**, and its insights are produced by sending entries to **OpenAI**. [C]

The catch: to find patterns, they **read the whole page**. One Morning Pages reviewer found the AI insights "not particularly useful or accurate". [B]

> **What it means for us:** "paper + patterns" alone is **not** our differentiator any more. What is different:
> - **The app never sees the pages.** Patterns come from **my own 10-second summary** (mood, themes, one idea), not from machine-reading private writing.
> - That matches the book's privacy ethic (pages aren't meant to be read, even by yourself, early on; `artists-way-practitioners.md` Finding 4) and lowers the "writing for the tag" risk compared with a full-page scan.
> - My own words are likely **more accurate** than inferred mood, which is the one complaint we found about AI insights.

### Finding 3: Nobody combines the course frame with daily tracking
- Apps have the **daily** loop and no course (no weeks, themes, artist dates, check-ins).
- Notion templates and printables have the **course** (12 weeks, artist dates, check-ins) and no daily ease or patterns: they are checkbox logs, as found in `artists-way-practitioners.md`. [C]
- The only official app (2012 Toolkit) had the course and artist dates, but I couldn't confirm it still exists. Its name now belongs to a **2025 book**, *The Artist's Way Toolkit*. [C]

> **What it means for us:** the brief's gap holds. The **artist date** in particular is tracked only by printables, templates and two hobby web apps.

### Finding 4: Streaks are the default, and 750 Words monetizes the anxiety
750 Words, Morning Pages and Daylio all use streaks. 750 Words offers a way to **"protect your streak"** after one missed day. Another Morning Pages reviewer complained that a change kept counting words toward the streak while the actual words vanished. [B/C]

> **What it means for us:** confirms the "no streak resets" decision (`user-complaints.md`). Our missed-day and missed-week handling (comeback moment, pause or continue) has no counterpart in the field.

### Finding 5: Two hobby projects are close to our idea
Two open-source phone web apps on GitHub pair a **paper notebook** with a phone tracker for artist dates and notes, storing data only on the device. [C]

> **What it means for us:** a signal that others feel the same need. Neither has a capture → pattern loop or early-weeks support. Worth a closer look in the walkthrough step for small UX ideas, not a threat.

### Finding 6: Low-friction mood logging is proven, and premium insights are what people pay for
Daylio's two-tap, no-typing logging is praised as the extreme low-friction end of the market; its deeper stats are paid, and users complain about features behind the paywall. [B/C]

> **What it means for us:** supports the "under 5 s tap, then optional ~10 s capture" approach. Daylio is a good **Mobbin reference** for the capture screen (Phase 3), but it's generic: it has no creative practice, themes or ideas.

### Finding 7: The paper journal is not enough even for its own users
Reviewers of the official *Morning Pages Journal* say there aren't enough pages for the whole program (one edition has 252 pages, about 84 days of three pages). It has instructions and quotes, but no week structure. [B]

> **What it means for us:** the paper notebook is the right place for the pages, but it gives no overview. That's the same gap as in my own attempts.

---

## Updated "What makes it different"
| Alternative | What it does | Gap we fill |
|---|---|---|
| Morning-pages apps (*Morning Pages*, *AM Pages*, *Pagi*, 750 Words) | Type your pages; word count; streaks; some AI insights | Paper-first; **no streak resets**; patterns from my own summary |
| **Scan-and-AI journals** (*Reflect*, *Journal Scanner*, Morning Pages' scan) *(new)* | Photograph paper pages; AI reads them, tags mood, answers questions | **The app never reads the pages**: I capture mood, themes and one idea in my own words |
| Mood trackers (*Daylio*) | Fast mood + activity logs, charts | Tied to the creative practice: themes and ideas → creative direction |
| Notion templates / printables | Static 12-week checklists | One tap on a phone; patterns build up; gentle missed-day handling |
| Paper journal / notebook | The pages, no overview | Patterns over time + the course frame |
| 2012 *My Artist's Way Toolkit* | Inspirations, notebook, artist dates | Status unconfirmed; the name is now a 2025 book |

---

## Candidates for decisions (for you to accept or change)
1. **Sharpen the positioning to "your pages stay private, even from the app".** The scan-and-AI apps take paper-first; our real difference is that patterns come from my own short words, never from reading the pages. Update the brief's differentiator table with the version above.
2. **No scan, OCR or AI reading of pages in the MVP, and say so on purpose.** Not a missing feature but a principle (book privacy, writing-for-the-tag risk, accuracy). Log it as a decision so it's in the case study.
3. **Add Daylio and the scan apps (Reflect, Morning Pages) to the Phase 3 Mobbin references,** for the capture screen and the pattern view, alongside the onboarding references.
4. **Verify before the case study:** current prices, the 2012 Toolkit's status, and whether "Morning Pages" (an app name already in use) affects our naming check.

---

## Sources
**Apps (C, B where reviews are quoted)**
- Morning Pages (Dahl & Sjöö): [App Store](https://apps.apple.com/us/app/morning-pages/id6738604034) · [FAQ](https://morningpages.app/faq/) · [site](https://morningpages.app/) · [studio](https://www.dahlsjoo.com/) · [Crunchbase (conflicting company info)](https://www.crunchbase.com/organization/morningpages) · [AppsHunter reviews](https://appshunter.io/ios/app/1223874080)
- [Morning Pages – Daily Journal (App Store)](https://apps.apple.com/us/app/morning-pages-daily-journal/id1223874080) · [TrendHunter on its AI insights](https://www.trendhunter.com/trends/aibased-journal)
- [Morning Pages: Diary & Journal (App Store)](https://apps.apple.com/us/app/id6714479684)
- [AM Pages (App Store)](https://apps.apple.com/us/app/am-pages/id1447417846)
- [Pagi – Morning Pages & Diary (App Store)](https://apps.apple.com/us/app/id1586446074)
- [Morning Pages for iOS & Mac (Literati)](https://www.literati.tools/morning-pages/en)
- 750 Words: [site](https://www.750words.com) · [FAQ](https://750words.com/faq) · [Working on V2 (pricing post)](https://medium.com/750-words/working-on-750-words-v2-321a7284153c) · [No Film School](https://nofilmschool.com/2012/10/free-platform-750-words-challenges-you-to-write-three-pages-every-day)
- Scan-and-AI journals: [Reflect (AlternativeTo)](https://alternativeto.net/software/reflect-ai-journal-diary/about/) · [Journal Scanner (App Store)](https://apps.apple.com/us/app/-/id6695735974) · [Journal Mate (App Store)](https://apps.apple.com/app/journal-mate/id1533808328)
- Daylio: [Headway review](https://makeheadway.com/blog/daylio-review/) · [Choosing Therapy review](https://www.choosingtherapy.com/daylio-app-review/) · [JustUseApp reviews (auto-generated summary)](https://justuseapp.com/en/app/1194023242/daylio-journal/reviews)

**Course trackers (C)**
- [The Artist's Way Companion (Notion template gallery)](https://www.notion.com/templates/the-artist-s-way-companion)
- [Hurley Winkler: 12-week printable tracker](https://hurleywinkler.gumroad.com/l/artists-way-tracker?layout=profile) · [Etsy printable toolkit](https://www.etsy.com/listing/4301253561/the-artists-way-toolkit-printable)
- Hobby web apps: [artist-way-companion](https://github.com/abasarcadi-ops/artist-way-companion) · [artist-way-compation](https://github.com/abasarcadi-ops/artist-way-compation)
- [Tu Camino del Artista: free 12-week online course](https://tucaminodelartista.com/en/the-artists-way.html)

**Official products (C, B)**
- 2012 app: [Adweek](https://www.adweek.com/performance-marketing/penguin-launches-artists-way-toolkit-app/) · [Shelf Awareness](https://www.shelf-awareness.com/theshelf/2012-02-02/app_of_the_day:_my_artist_s_way_toolkit_app.html) · [Publishers Lunch](https://lunch.publishersmarketplace.com/2012/01/enews-penguin-launches-mobile-platform-self-publishing-capabilities-from-nelson-literary-agency/) · [Big Girl Blue review (2012)](https://biggirlblue.com/2012/03/10/the-artist-way-toolkit-app-review/)
- 2025 book with the same name: [Macmillan](https://us.macmillan.com/books/9781250344977/theartistswaytoolkit/)
- Morning Pages Journal: [Julia Cameron Live](https://juliacameronlive.com/book/the-artists-way-morning-pages-journal) · [NetGalley](https://netgalley.com/catalog/book/99993) · [Walmart (page count)](https://www.walmart.com/ip/250821)
