# Asttarte Deva Healing Wellness Center

Static port of [the Wix site](https://asttartedeva.wixsite.com/centerforhealingarts) for **Cloudflare Pages**.

## Stack

- Semantic HTML + CSS (no framework)
- Vanilla JS (mobile nav only)
- Cloudflare Pages (`_headers`, `_redirects`, `wrangler.toml`)
- Assets mirrored from the live Wix media CDN at build time of this repo

## Local preview

```bash
cd astartte-sites
python3 -m http.server 8787
# open http://127.0.0.1:8787
```

Or with Wrangler:

```bash
npx wrangler pages dev .
```

## Deploy to Cloudflare Pages

1. Push this repo to GitHub (already: `kevinbaluha/astartte-sites`).
2. Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → Connect GitHub.
3. Select `astartte-sites`.
4. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (repo root)
5. Save and deploy.
6. Optional: attach custom domain `centerforhealingarts.net`.

CLI deploy (if `wrangler` is logged in):

```bash
npx wrangler pages deploy . --project-name=astartte-sites
```

## Content notes

- Contact, phone, email, Calendly, and service copy were taken from the public Wix site (Oct 2026).
- Intake uses a `mailto:` fallback; swap for Cloudflare Workers / Formspree before production traffic.
- Blog was not ported (Wix CMS). Add later if needed.
- Pricing figures appear only where published on the source Reiki page.

## Source map

| Wix path | This site |
|---|---|
| `/` | `/` |
| `/services` | `/services/` |
| `/reiki-and-energy-healing` | `/services/reiki-and-energy-healing/` |
| `/massage-therapy` | `/services/massage-therapy/` |
| `/somatic-stress-release` | `/services/somatic-stress-release/` |
| `/breathwork` | `/services/breathwork/` |
| `/yoga-and-meditation` | `/services/yoga-and-meditation/` |
| `/coaching` | `/services/coaching/` |
| `/tarot-astrology-readings` | `/services/tarot-astrology-readings/` |
| `/about-4` (Sound Healing) | `/services/sound-healing/` |
| `/reiki` | `/services/reiki-traditions/` |
| `/holistic-health` | `/services/holistic-health/` |
| `/eft` | `/services/eft/` |
| `/contact` | `/contact/` |
| `/spiritual-holistic-form` | `/intake/` |
