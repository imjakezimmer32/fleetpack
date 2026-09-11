# FleetPack Pack #01 — Landing Page

Static landing page for **FleetPack — Agent Ops Research Brief (Pack #01)**.

Single-file HTML + CSS. No build step.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Landing page (hero, included, audience, install, FAQ, footer) |
| `preview.html` | Optional: add later for “Preview the example brief” (linked from CTA) |

## Deploy to Cloudflare Pages

You already have Cloudflare connected. Use either path below.

### Option A — Dashboard (fastest)

1. Open [Cloudflare Dashboard](https://dash.cloudflare.com) → **Workers & Pages** → **Create** → **Pages**.
2. Connect the repo that contains this `landing/` folder (or upload assets).
3. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** path to this folder, e.g. `fleetpack/landing` (or `.` if the repo root *is* this folder)
4. Save and deploy. Pages will serve `index.html` at the project URL.
5. Optional: attach a custom domain under the project’s **Custom domains** tab.

### Option B — Wrangler CLI

From this directory (or with the correct path):

```bash
npx wrangler pages deploy . --project-name=fleetpack-pack-01
```

- First run may prompt you to create the Pages project.
- Re-run the same command to publish updates.
- Ensure you’re logged in (`npx wrangler login`) with the Cloudflare account that already has Pages connected.

### After Polar is connected

Replace the Buy button `href="#"` in `index.html` with the Polar checkout URL, and remove or update the note *“Checkout link lands when Polar is connected”*.

### Preview CTA

The secondary button points at `./preview.html`. Add that file when the example brief is ready, or change the href to your preferred preview path.
