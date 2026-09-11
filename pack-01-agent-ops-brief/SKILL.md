# Agent Ops Research Brief

> FleetPack Skill · Pack #01 · v1.0.0  
> Install: drop this folder into `.cursor/skills/` (or paste into a project rule / custom skill).  
> Brand: FleetPack — The Dude runs ops so you don't have to.

## Purpose

Teach any agent how to run a **weekly research → synthesis → one-page brief** pipeline.  
Output is a single, scannable ops brief a human can act on in under five minutes — not a wall of links.

Use this skill when the user asks for:
- A weekly / recurring research brief
- Competitive or landscape scan
- "What's new in X this week?"
- Source-backed synthesis with a clear recommendation

## Non-goals

- Financial advice, investment tips, or crypto signals
- Scraping private / authenticated systems
- Dumping raw search results without synthesis
- Long reports (keep the deliverable to **one page**)

---

## Pipeline (follow in order)

### 1. Scope lock (60 seconds)

Before searching, confirm or infer:
| Field | Example |
|-------|---------|
| **Topic** | MCP marketplace landscape |
| **Time window** | Last 7 days (or stated range) |
| **Audience** | Founder / ops lead / eng lead |
| **Decision** | What should they do / watch / ignore? |
| **Out of scope** | Anything the brief must not cover |

If the user gave a vague ask, state your assumed scope in one sentence and proceed. Do not stall.

### 2. Collect (web search + hygiene)

- Run **3–8 targeted searches** (not one vague query). Mix: product names, "announcement", "pricing", "open source", year.
- Prefer **primary sources**: official blogs, docs, GitHub releases, reputable trade press.
- For each candidate source capture:
  - Title · URL · Publisher · Date · Claim in one line
- **Source hygiene rules**
  - Discard undated rumor threads unless corroborated by ≥2 independents
  - Flag paywalled or registration-gated items as `[gated]`
  - Never invent URLs, quotes, or dates
  - Prefer 2025–2026 material for "current landscape"; label older items as `[background]`

### 3. Scorecard (force ranking)

Score each finding **1–5** on three axes (write the numbers; don't just vibe):

| Axis | Meaning |
|------|---------|
| **Signal** | How much this changes the landscape |
| **Confidence** | Source quality + corroboration |
| **Actionability** | Can the reader do something this week? |

**Priority score** = `(Signal × 2) + Confidence + Actionability` (max 15).  
Keep the top **5–7** items for the brief; park the rest under "Parking lot" (one line each).

### 4. Synthesize

Write for a busy human:
- Lead with **what changed** and **why it matters**
- Group findings into 2–4 themes (not a chronological dump)
- Call out contradictions explicitly ("A says X; B says Y")
- Separate **facts** from **FleetPack take** (opinion)

### 5. Deliver (one-page brief)

Produce exactly the format in **Deliverable format** below.  
Hard length target: **≤ 450 words** for the main body (excluding source list).

---

## Deliverable format

Copy this skeleton every time:

```markdown
# Ops Brief: {Topic}
**Window:** {start} → {end} · **Prepared:** {date} · **Audience:** {role}

## TL;DR
{3 bullets max. Decision-oriented. No throat-clearing.}

## What moved
| # | Finding | Priority | So what? |
|---|---------|----------|----------|
| 1 | … | {score}/15 | … |
| 2 | … | … | … |
| 3 | … | … | … |

## Themes
### {Theme A}
{2–4 sentences + one concrete implication}

### {Theme B}
…

## Watch / Act / Ignore
| Bucket | Item | Why |
|--------|------|-----|
| **Act this week** | … | … |
| **Watch (30d)** | … | … |
| **Ignore for now** | … | … |

## FleetPack take
{4–6 sentences. Opinionated but honest. No hype.}

## Sources
1. [{Title}]({URL}) — {Publisher}, {Date} — {one-line claim}
2. …

## Parking lot
- {Low-priority note}
```

---

## Quality bar (self-check before shipping)

- [ ] Scope stated; time window clear
- [ ] ≥3 independent sources cited with dates
- [ ] Scorecard numbers present (not just adjectives)
- [ ] Act / Watch / Ignore is non-empty and specific
- [ ] No secrets, no private URLs, no financial advice
- [ ] Main body fits one page / ≤450 words
- [ ] Tone: clear, dry-humor OK, never corporate sludge

---

## Recurring / weekly mode

When asked to run this weekly:
1. Reuse last brief's **Watch** items as this week's seed queries
2. Diff: open with "Since last brief…" (2–3 bullets of deltas only)
3. Archive prior briefs as `brief-YYYY-MM-DD.md` if the user wants a trail

---

## Voice (FleetPack / The Dude)

- Straight talk. Short sentences.
- "Here's what matters. Here's what doesn't."
- Light personality; zero condescension.
- Never name-drop unrelated products or client work.

---

## Failure modes → fixes

| Failure | Fix |
|---------|-----|
| Brief is a link dump | Cut to top 5 by priority; rewrite So-what column |
| Vague recommendations | Rewrite Act items as verbs + owners + timeframe |
| Stale sources | Re-search with current year; demote old to background |
| Scope creep | Move extras to Parking lot; protect the one-page limit |

---

## Install (Cursor)

1. Copy this entire `SKILL.md` into your project as  
   `.cursor/skills/agent-ops-research-brief/SKILL.md`  
   (or merge the pipeline into your team's custom instructions).
2. In chat: `@agent-ops-research-brief` (or invoke by name) and give a topic + window.
3. Optional: pin a recurring prompt —  
   `Run Agent Ops Research Brief for {topic}, last 7 days, audience = {role}.`

That's the whole skill. Keep it tight. Ship the brief.
