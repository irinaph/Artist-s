# Designing with Claude Code: The Lecturer's Process

**Source:** DEV.BG AI Workshops recording (3h40m, Bulgarian). Lecturer: Philip (Phil) Rusev, Principal UX Designer at Progress (AI division).
**His claim:** he shipped 5+ features (15+ screens and a small desktop app) in 3 months without opening Figma, working with Claude Code from research through design to a pull request.
Timestamps `[h:mm]` point to the recording and to `transcript-bg.md`.

---

## Part 0: Concepts to understand first  `[0:16–0:26]`

| Concept | What it means for a designer |
|---|---|
| **LLM ("the brain")** | Only reads and writes. Reading, thinking (hidden writing), writing and reading images all cost **tokens** (pieces of words). |
| **Tools** | Built-in "hands": read, write, run, search. The model can edit files directly instead of you copy-pasting its output. |
| **Context** | Everything the model sees: system prompt, `CLAUDE.md`, memory, your prompts, tool results, skill names, MCP tools. |
| **Context window** | Like human working memory. When it fills, older content gets compacted (summarized). **Managing context is the #1 skill.** |
| **CLAUDE.md** | A text file the agent reads on *every* turn, like your own system prompt. Keep it short. |
| **Skills** | Extra instruction files the agent loads only when needed. |
| **MCP / Connectors** | A standard "common language" that lets Claude talk to other apps (Figma, GitHub, Mobbin, Gmail, browser). |
| **Harness** | The app around the model (Claude Code) that provides tools, context and the loop. |
| **Agent** | Model + harness running in a **loop** until it decides it's done. It is **non-deterministic**: the same prompt gives different answers. That's a feature you can exploit. |
| **Subagents** | Parallel helpers that each start with an **empty, fresh context** and a short brief. |

Mental model: the agent is a very smart new hire. You can't change its intelligence, but you can shape its context, skills and processes.

---

## Part 1: Setup  `[0:26–0:47]`

1. **Plan:** none of this works on the Free plan; you need at least **Pro**.
2. **App:** use the **Claude desktop app → Code tab** (terminal or VS Code also work).
3. **Work in a folder.** Claude Code works on a folder you choose. That folder *is* the context, which is the big difference from regular Claude chat, where memory from every past chat leaks in.
   - Demo: in chat, "who am I?" returns his whole bio from memory. In Claude Code with a folder, it only knows the project.
4. **Watch the context.** Type `/` for the command menu. `/context` shows what's filling memory; `/compact` compresses it.
5. **Create a `CLAUDE.md` with a personality.** Prompt: *"Write a CLAUDE.md file, give it a personality of a product designer."* Connect the folder, ask "who are you?", and it answers as a senior product designer, still Claude underneath.
   - Keep `CLAUDE.md` short; it's read every turn, and a long one hurts decisions.
6. **Connect tools:** **Customize → Connectors** (Mobbin, Figma, GitHub, Gmail…). You need an account in both apps. You can also just ask Claude in chat to set it up.
   - Customize has 3 areas: **Skills**, **Connectors** (MCPs) and **Plugins** (bundles of skills + MCPs).

---

## Part 2: Skills  `[0:46–1:04]`

1. Ask for a "quick research" and Claude improvises; ask for "in-depth" and it may pick Anthropic's **deep-research** skill on its own.
2. **Create your own skill by prompting:**
   > Create the following skill in this folder: name `pattern-research`. Description: quick UI pattern research with Mobbin; use when asked for research patterns or examples of how other apps solve a UI problem. 1) Use the Mobbin MCP only, no web search. 2) Split the pattern into 3 angles and send one subagent per angle in parallel. 3) Each returns max 3 examples (app, screenshot, one line on what works). 4) Combine everything into one short file in `research/`. 5) Keep it quick, not deep. 6) Your output is an HTML artifact.
   - **Always state the expected output** (here: an HTML artifact).
   - It is saved in a hidden folder: `.claude/skills/pattern-research/SKILL.md`.
3. Run `/reload-skills` (or start a new session) so it shows up as a `/pattern-research` command.
4. **To guarantee a skill is used**, call it as a slash command at the start of your prompt; otherwise the agent may skip it.
5. **Scope:** skills in Customize work in every project; a skill inside a project folder works only in that project.
6. **Many skills (teams use 100+)?** Organize them like a book's table of contents: group by category (research, design, front-end) and reference the outline from `CLAUDE.md`, with a short title and a "when to use" description for each.
7. **Artifacts** are interactive, shareable HTML pages (private by default; can be shared publicly). His bigger table-pattern research covered 18 products, 24 flows and 111 screens, and took ~20 min.

---

## Part 3: The end-to-end process (case study: Rallly)  `[1:04–3:10]`

**Rallly** is an open-source scheduling-poll app. He chose it because it's simple and its code is public on GitHub. Metrics, PM and persona were invented to make it realistic.

### Phase A: Discovery (one session, "Discovery")

1. **Get the real product locally.** `[1:06]` Ask Claude to clone the repo to your desktop and run it on a local server. This takes a snapshot of the code at one point in time, so others' changes don't break your work.
2. **"Chat with the product."** `[1:10]` With the repo, the agent becomes a wiki you can question: *"Why can't I create an event?"* (Answer: an event is a poll whose date got confirmed. Note that as a possible UX issue.)
   - Since it's your local copy, you can ask it to **make you a paid user** or **seed fake data** (many polls, many members) to experience every state.
3. **Frame the problem.** `[1:09]` The (invented) PM says free→paid conversion dropped from **6.8% to 3.9%** among users who made 2+ polls in 30 days.
4. **Research with subagents.** `[1:17]` *"Browse online, forums, reviews, user-generated complaints about this tool."* Claude launched parallel subagents (forums, GitHub issues).
5. **Competitor analysis.** `[1:21]` *"How easy is it to switch to another tool?"* → `competitors.md`. Insight: **nobody else charges for picking the final slot.**
6. **Persona.** `[1:22–1:26]` Reason it out together: who needs this? People coordinating 8–12 people who aren't colleagues (otherwise they'd use a shared calendar). → **Yana, a small-agency event planner** (vendors, caterers, AV crews). The persona is focused only on her world as it relates to this task, not demographics. → `persona.md`
7. **User journey with a mental model.** `[1:26–1:29]` For each step: **what actually happened, what she expected, what she thinks, what she feels.** → `journey.md`
8. **Persona walkthrough of the real app.** `[1:29–1:33]` Prompt idea: *"Start a fresh session in the app, imagine you are Yana, walk through every journey step, stop at each one, take a screenshot and analyze what she thinks and feels."* → an artifact, "Yana's Journey Through Rallly". Finding: Pro badges and payment requests appear before she's even created anything.
9. **Be critical.** Read everything; don't accept output blindly. In real life, feed it real data, interviews and tests.

*(Break `[1:34–1:45]`.)*

10. **Fresh eyes with 5 subagent designers.** `[1:48–1:52]` *"Spawn 5 independent product designers. Each gets the PM's brief, the persona and the walked journey (not our notes or parked ideas) and returns ideas."* → `synthesis.md`
    - **Why subagents:** no accumulated context, so no bias or "context fatigue."
    - **Why 5:** non-determinism gives variety. All 5 suggested a **free trial**, the same idea he'd had himself.
11. **Feasibility check with the code.** `[1:53–1:55]` *"What if we do a free trial? Give me a real estimate."* The agent found a `trial` column **already in the backend**, just not in the front-end. That means low effort, and the product is already heading this way. It's a technical-feasibility conversation without waiting for engineers.
12. **Pattern research with Mobbin.** `[1:56–2:03]` 3 parallel researchers, one per moment: **before the ask / trial start / trial end**. → artifact "Free-to-Paid Patterns". Good: contextual upgrade prompts and trial notices with an end date. Bad: the same generic plans popup everywhere (which Rallly does).
13. **Trim the scope.** `[2:03–2:05]` Drop valid but off-focus issues (for example, "add an answer for someone").
14. **Hand off when context gets heavy.** `[2:05]` At ~76% context: *"Make a handoff for a new session."* → `HANDOFF.md` + `project-scope.md` + a ready-to-paste first prompt.
    - **Why a new session:** 1,000 messages boil down to 5–8 decision files. A clean start beats auto-compaction, where *it* decides what to keep. All sessions share the same folder, so files carry the context.

### Phase B: Design (new session, "Design")  `[2:06–2:29]`

15. **Design canvas inside Claude Code.** No separate tool and no Figma: the canvas has the full context plus access to the product's code, so it **builds variations using the product's real design system** automatically.
16. **Versioning rule:** *"Don't overwrite; create a new version/row for each round of feedback"* so you can trace how you got there.
17. **Explore variations** of copy, buttons and layouts. Boards can be **playable prototypes**.
18. **Re-ground in the real flow.** `[2:13]` When stuck on a modal: *"Go back to the app and put screenshots of every step on the canvas."*
19. **Evaluate prototypes with subagents.** `[2:17]` 5 prototypes → *"10 agents, 2 per idea, tell me what you think of the mechanisms."* Like grabbing a designer in the office for fresh eyes.
20. **The key decision** `[2:18–2:20]`: users were asked to pay in two places (settings toggles + share dialog). Merge them into **one choice, once**: after creating the poll, a step asks *"continue Free, or Pro with 14 days free?"*
    - No "brilliant ideas from nowhere": try many things, look at many references, and trust the gut that says "not good enough yet."
21. **Mobbin for UI (not UX).** `[2:21–2:27]` *"Find 3 references from Mobbin and use them."*
    - **Tip:** have it **copy one reference**, not mash 10 together (that produces a mess). Divide and conquer is OK: one reference per section.
    - The narrower the focus, the better the design quality.
22. **Parallel backend work.** `[2:29–2:32]` From the design session: *"Can we start backend in a separate session?"* → a new session on a branch → a written report back.

### Phase C: Front-end build (new session, "Front-end")  `[2:32–3:00]`

23. **Let the agent write the prompts.** He never writes skills, `CLAUDE.md` or handoff prompts by hand: discuss → agent drafts → review → feedback → repeat. Trim the wordiness.
24. **The repo *is* the design system.** `[2:36]` *"How do we make sure you don't write custom code?"* The answer: Rallly's repo has
    - a `CLAUDE.md` rulebook (copy style, sentence case…)
    - shared UI component packages (~60: buttons, cards, switches)
    - shared styles CSS (tokens)
    - existing pages to reuse
    - built-in checks (lint, type-check, structure, i18n, tests)
25. **Ask for gaps up front.** `[2:44]` *"I expect gaps. Find things we've missed."* For example, a removed element still exists elsewhere.
26. **Verify like a designer.** Open the live build, click through every state, and **Inspect element** in the browser to confirm tokens and text styles are used.
27. **Lesson from real engineers:** `[2:40]` his first hand-off was full of **mock data** the engineer had to hunt down and wire to real APIs. Build on real data and APIs.
28. **Evaluation skill (evals).** `[2:41–2:43]` Collect engineers' feedback → turn it into an **eval skill** → it runs a **fresh subagent with no context** that judges the output only against criteria ("7/10; to reach 9.5 fix X, Y, Z") → fix → re-run. Share the skill with engineers so they can improve it.

### Phase D: Shipping via GitHub  `[3:00–3:10]`

29. **Git basics:** a **repository** holds the code; **issues** are like Jira tickets; **main** is the live branch. You **branch** (take a "moment" copy), work, then open a **pull request** to **merge** back. Figma branching is the same idea.
30. All done from Claude Code; he never touched GitHub directly. Claude opened a **draft PR** (drafts don't notify anyone or get auto-reviewed).
31. **Merge conflict reality:** in ~2 weeks upstream had **146 commits**. One feature he'd put in the trial became free for everyone, and React hooks changed, so the merge wasn't feasible. The PR stayed a draft and was closed. The principle still stands.
32. **Ask "explain it simply,"** then explain it back in your own words to check your understanding.

---

## Part 4: Making a design system agent-ready  `[2:49–2:59]`

1. **A solid design system in code:** components, tokens and styles, well connected, and one you're happy with yourself. Code and Figma must not drift apart.
2. **Usage rules:** when to use each piece and **when never to** (like Material or Apple docs). For big systems, split them into skills or files per component plus an outline; his company's engineers built a **plugin**.
3. **Evals:** an independent agent checks output against clear criteria.
- **Connecting it:** a GitHub repo (get read access), an **npm** package installed locally, or Figma via MCP (needs a lot of work, not one prompt).
- **DESIGN.md:** a single-file design system for small sites or MVPs. Sites like "DESIGN.md examples" have files extracted from well-known brands (e.g. Airbnb: "Rausch red is a decorative accent; never promote it to primary"). Download one you like and make it yours.

---

## Part 5: Principles to take away

- **Control context:** one folder per project, separate sessions per phase, file-based handoffs, and a lean `CLAUDE.md`.
- **Write decisions to files** (`.md`) so any session can pick them up.
- **Use subagents** for parallel research and for **unbiased fresh-eyes reviews**; more agents surface more outliers. AI gives "the best of average," and average design isn't enough.
- **Give agents goals + success criteria, not step-by-step instructions** (like good user stories).
- **Build `CLAUDE.md` and skills *during* real work, not upfront.**
- **Export the chat transcript** of finished projects and analyze it with another agent to discover your *real* process; you'd unknowingly misdescribe it otherwise.
- **Copy one strong reference** for UI; use Mobbin for visual patterns and competitor docs for deep UX logic.
- **Always stay critical**; keep the human in the loop.
- **Pushing for change at work:** don't argue, build a small proof and show it. Meet engineers 1:1, not in a big meeting.
- **Portfolio challenge:** pick an open-source product, run this process, and open a real PR.

## Q&A highlights  `[3:19–3:39]`
- **Testing:** sales-call shadowing + competitor docs. For user tests, build a realistic **artifact prototype** of only the flow under test, share the link and use it in a user-testing tool.
- **Without an open-source repo:** ask your company for **read access** to the repo; that's enough to experiment.
- **Eval isolation:** location doesn't matter; launch the eval as a **subagent** (empty context). Gate evals by phase (only in the build phase). Run many in parallel for statistical breadth.
- **Stakeholder criteria:** collect them over time into a skill, then run "virtual stakeholder" reviews early.
