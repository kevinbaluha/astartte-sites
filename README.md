**Primary domain:** AsttarteDeva.com (centerforhealingarts.net may forward).

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

### Automated (GitHub Actions) — preferred

Workflow: [`.github/workflows/publish.yml`](.github/workflows/publish.yml)

| Event | Result |
|---|---|
| Push to `main` | Production deploy (`astartte-sites`, branch `main`) |
| Pull request | Preview deploy on the PR branch |
| **Actions → Publish → Run workflow** | Manual deploy |

**One-time setup**

1. Cloudflare Dashboard → **My Profile** → **API Tokens** → **Create Token**
   - Use template **Edit Cloudflare Workers** (includes Pages), or custom token with:
     - Account · Cloudflare Pages · Edit
     - Account · Account Settings · Read (optional, for account listing)
2. Copy **Account ID** from the right sidebar of any Workers/Pages overview page.
3. In GitHub repo **Settings → Secrets and variables → Actions**, add:
   - `CLOUDFLARE_API_TOKEN` — the token
   - `CLOUDFLARE_ACCOUNT_ID` — the account id
4. (Optional) Pre-create the project once:
   ```bash
   npx wrangler pages project create astartte-sites --production-branch=main
   ```
   If the project does not exist yet, the first successful Actions deploy with a valid token usually creates it when using `pages deploy`.
5. Push to `main` or run the workflow manually.

Deployment URL and alias are written to the Actions job summary.

### Manual CLI

```bash
npx wrangler login   # once, interactive
npx wrangler pages deploy . --project-name=astartte-sites --branch=main
```

### Dashboard Git integration (alternative)

You can instead connect the repo in **Workers & Pages → Create → Pages → Connect to Git** with:

- Framework preset: **None**
- Build command: *(empty)*
- Build output directory: `/`

Do **not** enable both Dashboard Git builds *and* this Actions workflow on the same project, or every push will double-deploy. Pick one.

## Content notes

- Contact, phone, email, Calendly, and service copy were taken from the public Wix site (Oct 2026), then updated with Asttarte’s intimacy and cacao pages.
- No intake form. Booking is Calendly; old intake URLs redirect to contact.
- Blog posts from the Wix site are under `/blog/`.
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
| `/spiritual-holistic-form` | `/contact/` |
