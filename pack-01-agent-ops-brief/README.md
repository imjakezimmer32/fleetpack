# Pack #01 — Agent Ops Research Brief

> Priced for the AI age — built with AI help, so you pay less.

**FleetPack** · Digital product for Cursor agents  
**Price:** $9 USDC (Solana) · **License:** Simple commercial (see below)

---

## What it is

A production-ready **Cursor skill** that teaches any agent how to run a weekly **research → synthesis → one-page brief** pipeline.

You get:
- Source hygiene rules (no rumor dumps)
- A forced scorecard so priorities aren't vibes
- A fixed one-page deliverable format your team can standardize on
- A fully worked example brief so you see the output shape before you run it. Open `EXAMPLE-BRIEF.md`.

The Dude's take: most "research" from agents is a pile of links. This pack makes the pile into a decision.

---

## Who it's for

- Founders and ops leads who want a **Monday morning one-pager**
- Agency / consultancy teams standardizing client (or internal) landscape scans
- Eng leads tracking tooling ecosystems (MCP, agents, IDEs, platforms)
- Anyone tired of re-prompting "please cite sources and keep it short" every week

**Not for:** day traders, crypto signal hunters, or anyone wanting financial advice. This pack won't do that — on purpose.

---

## What's included

| File | Role |
|------|------|
| `SKILL.md` | The installable Cursor skill (pipeline + format + quality bar) |
| `EXAMPLE-BRIEF.md` | Fully worked sample: MCP marketplace landscape (2026) |
| `LISTING.md` | Marketplace / store copy if you list elsewhere |
| `CHANGELOG.md` | Version history |
| `README.md` | You are here |

---

## Install (Cursor) — ~2 minutes

1. In your project (or global Cursor config), create:
   ```
   .cursor/skills/agent-ops-research-brief/
   ```
2. Copy `SKILL.md` into that folder (keep the filename `SKILL.md`).
3. Restart Cursor chat or reload skills if your build requires it.
4. Invoke with a clear ask, for example:

   > Run **Agent Ops Research Brief** on "{topic}" for the last 7 days. Audience: founder. Decision: what to watch vs ignore.

5. Optional: save a recurring snippet in your team docs so every Monday uses the same scope fields.

**Copy-paste install tip:** If your Cursor version uses project rules instead of skills folders, paste the pipeline sections from `SKILL.md` into `.cursor/rules/` as a dedicated rule named `agent-ops-research-brief`.

---

## 60-second demo

1. Open a Cursor chat in any repo.
2. Paste or invoke the skill.
3. Say:  
   `Agent Ops Research Brief — topic: MCP marketplace landscape, window: last 30 days, audience: indie founder shipping a digital product.`
4. Expect: TL;DR → scored findings table → Act/Watch/Ignore → sources with dates.
5. Compare shape to `EXAMPLE-BRIEF.md` in this pack. Same skeleton, your topic.

If the output is a link salad, the skill's quality bar wasn't followed — nudge: *"Apply the scorecard and keep the body under 450 words."*

---

## License (simple commercial)

**You may:**
- Use this pack inside your company / team / personal projects
- Modify the skill text for internal workflows
- Run the pipeline for clients as part of *your* services (the brief is your work product)

**You may not:**
- Resell, republish, or redistribute this pack (or a thinly rebranded copy) as a competing digital product
- Share the raw pack files publicly (GitHub public repo, free download sites, etc.)

No warranty. Ships as-is. If it saves you an hour a week, The Dude did his job.

© FleetPack. All rights reserved for the pack contents; your generated briefs are yours.

---

## Support / vibe

FleetPack builds small, sharp agent packs — not bloated courseware.  
Buy: 9 USDC on Solana (see `landing/BUY-USDC.md`).  
Keep the brief to one page. That's the whole product philosophy.
