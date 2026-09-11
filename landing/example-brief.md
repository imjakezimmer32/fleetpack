# Ops Brief: MCP Marketplace Landscape
**Window:** 2026-08-01 → 2026-09-11 · **Prepared:** 2026-09-12 · **Audience:** Indie founder shipping agent tooling

## TL;DR
- MCP (Model Context Protocol) skill/tool marketplaces are consolidating around a few host surfaces — Cursor-style skill folders, Claude/Anthropic connector catalogs, and open registries on GitHub.
- Distribution still beats polish: packs that install in under two minutes and show a worked example convert better than feature-heavy dumps.
- Act: ship one tight pack with clear license + example output; Watch: host-native discovery APIs; Ignore: "universal agent app store" vapor for now.

## What moved

| # | Finding | Priority | So what? |
|---|---------|----------|----------|
| 1 | Host products increasingly treat **skills / tools as first-class installables** (folder drop or one-click connector), not just prompt paste. | 13/15 | Package as an install unit, not a blog post. |
| 2 | Open MCP server lists and community registries grew; quality variance is huge — buyers look for **hygiene + demo artifact**. | 12/15 | Include EXAMPLE output; state non-goals. |
| 3 | Pricing for digital agent packs clusters **$19–$49** for single-purpose skills; bundles go higher. | 11/15 | $29 single-pack is a sane default. |
| 4 | "Marketplace" UX is fragmented: some hosts curate; others are BYO Git folder. Cross-host one-click is rare. | 10/15 | Don't wait for a universal store — sell direct + list where you can. |
| 5 | Buyers complain about **prompt packs without a pipeline** (no scorecard, no format, no recurrence). | 10/15 | Differentiate on process, not adjective density. |

*Priority = (Signal × 2) + Confidence + Actionability.*

## Themes

### Host-native beats "yet another directory"
Discovery is happening inside the tools people already open daily. A beautiful standalone directory helps SEO; install friction decides retention. Packs that map to the host's skill/connector model win.

### Trust theater → trust artifacts
Screenshots of chat are weak proof. A full sample brief, changelog, and explicit license reduce refund risk and support load. Source-dated research norms (even in the skill itself) signal seriousness.

### Small packs, clear edges
The market rewards narrow jobs ("weekly research brief") over mega-bundles that try to replace an entire ops org. Edge cases belong in a parking lot — not in v1 scope.

## Watch / Act / Ignore

| Bucket | Item | Why |
|--------|------|-----|
| **Act this week** | Publish Pack #01 with SKILL + EXAMPLE + license; price $29 | Matches buyer expectations and install path |
| **Watch (30d)** | Host APIs / submission guidelines for curated skill catalogs | May unlock distribution without rebuilding the product |
| **Ignore for now** | Building a multi-vendor "app store" frontend | Premature; hosts own discovery |

## FleetPack take

The MCP marketplace story in mid-2026 is less "there's one App Store" and more "every serious host wants installable capabilities." That favors people who ship **boring, repeatable pipelines** wrapped as skills. If your pack needs a webinar to explain, it's not a pack — it's a course. Keep the brief to one page. Keep the skill copy-paste installable. Charge enough that you can maintain it. Everything else is noise.

## Sources
1. [Model Context Protocol specification / docs](https://modelcontextprotocol.io) — MCP project, ongoing — Defines tools/resources/prompts model hosts implement.
2. [Anthropic — MCP and connector announcements](https://www.anthropic.com/news) — Anthropic, 2025–2026 — Host-side connector/catalog direction (verify latest post dates when refreshing).
3. [Cursor docs — Skills / rules](https://docs.cursor.com) — Cursor, 2025–2026 — Skill-folder and rules patterns for installable agent behavior.
4. [Awesome MCP / community server lists on GitHub](https://github.com/topics/mcp) — Community, 2025–2026 — Volume of MCP servers; quality uneven; use as landscape signal only.
5. Public indie pricing pages for AI prompt/skill packs — Various creators, 2025–2026 — Observed $19–$49 band for single-purpose digital packs `[background]`.

*Note: Refresh URLs and dates on each weekly run; never invent citations.*

## Parking lot
- Deep dive on enterprise SSO for connector marketplaces (out of scope for indie pack sellers).
- Comparison of RPC vs REST transport choices inside MCP (implementer concern, not buyer brief).
- Localization of skill packs (interesting; not this window).
