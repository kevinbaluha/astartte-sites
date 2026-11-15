# Action Plan: Building Greater Trust & E-E-A-T for Asttarte Deva Healing Wellness Center

**Prepared for Asttarte Deva**  
**Date:** Current (on seo-review-oct2026 branch)  
**Goal:** Strengthen Experience, Expertise, Authoritativeness, and Trustworthiness (E-E-A-T) signals across the web. This improves rankings (especially local pack and organic), AI Overviews citations, user confidence, and long-term authority. Focus on verifiable, consistent signals that local service businesses like yours can control better than national competitors.

**Important Note on Redirects (from your request):**  
We will **not** apply blanket 301 redirects for old paths that are referenced by high-trust external sites/directories/profiles. These sites contribute citation strength, prominence, and backlink-like signals. 

Priority order:
1. Update the external source to point to the **current correct URL** (e.g., change old /tantra-coaching or /coaching to /services/intimacy-coaching/).
2. Where we cannot update the source quickly (or for UX to avoid 404s that hurt trust), keep the old path serving **relevant content** (not a blind redirect) or a clear "This service is now part of..." page with strong trust signals (bio, boundaries, testimonials, schema).
3. Only use 301s for low-trust or purely internal/historical references. We will audit and selectively remove/comment the new external-specific redirects in `_redirects` for high-trust sources.

See `docs/external-redirects.csv` for the full list with "Trust Source?" notes and recommended actions. High-trust examples: Yelp, Alignable, about.me, Fairies in America, Amazon author page, established directories.

**Current High-Trust Referring Sites (from indexed references):**
- Yelp listings (review/citation strength)
- Alignable (business directory)
- about.me (professional profile)
- Fairies in America (niche directory with links to AsttarteDeva.com and CenterforHealingArts.net)
- Amazon author/books pages (authoritativeness)
- Linktree (her own, but aggregator)
- Her own Wix sites and Mailchimp (historical — 301s generally okay here as internal content move; update if possible)
- YouTube channel (her own — update descriptions)
- Others: Instagram, X, Pinterest, occasional Craigslist mentions via social.

## Phase 1: Immediate Redirect & Source Audit (1-2 weeks)
1. Review `docs/external-redirects.csv`.
2. For each high-trust site:
   - Log in / contact and update any links/descriptions to current paths (e.g., /services/intimacy-coaching/, /services/breathwork/, /services/reiki-and-energy-healing/).
   - Standardize name to "Asttarte Deva Healing Wellness Center" or exact branding.
3. In the repo (on this branch or after merge): Comment out or remove 301 rules for paths tied to high-trust sources. Replace with content pages if the old URL has value.
4. Test live after changes: Use `curl -I https://www.asttartedeva.com/[old-path]`.
5. Submit updated URLs for indexing in Google Search Console.

**Deliverable:** Updated `_redirects` (selective) + list of updated external sources.

## Phase 2: Google Business Profile (GBP) – Highest Impact Trust Signal (~32% local pack weight)
1. Claim/verify the profile at business.google.com (use exact NAP: Asttarte Deva Healing Wellness Center, Manayunk/Philadelphia address, 215-326-9641, AsttarteDeva@gmail.com).
2. Choose primary category carefully (e.g., "Holistic Medicine Practitioner" or most specific matching "Wellness Center" + services like "Massage Therapist" or "Life Coach").
3. Complete every field: Hours (accurate, including "open now" signals), photos (quiet, professional, before/after if appropriate, team if any), services list, attributes.
4. Post regularly (updates, offers, tips — not salesy).
5. Enable messaging and Q&A if available; answer promptly.
6. Add service areas (Manayunk, Northern Liberties, Lambertville NJ, online).
7. Request reviews from every client (see below).

**Target:** 100% profile completeness, 4.5+ stars with recent reviews.

## Phase 3: Reviews & Social Proof (Critical for Trust & Prominence, ~20%+ weight)
1. Systematically ask happy clients for reviews on Google (primary), Yelp, and Alignable right after sessions.
2. Provide easy links (e.g., via Calendly confirmation or email).
3. Respond to **every** review within 48 hours (positive and negative) — thank, address specifics, show care.
4. Collect video or written testimonials for the website (with permission; anonymize if needed).
5. Display 3-5 strong, recent testimonials on homepage and service pages (with context like "after 3 sessions...").
6. Avoid incentivizing or fake reviews (Google penalizes).

**Goal:** Steady flow of authentic reviews. Track recency and response rate.

## Phase 4: Citation Consistency (NAP Across Web)
1. Audit all listings using the CSV + tools like Whitespark or manual search.
2. Ensure **exact match** everywhere: "Asttarte Deva Healing Wellness Center", full address, phone, email, website.
3. Update high-trust sites first (Yelp, Alignable, about.me, Fairies in America, Amazon).
4. Add to more relevant directories: Local Philly wellness/health lists, holistic practitioner directories, BBB if fits.
5. Use consistent categories/descriptions that match current services (no outdated "tantra" or "plant medicine" if not primary now — align with brand separation: wellness center for services, Love as Medicine for deeper/writings).

**Tool tip:** Search "Asttarte Deva" + location in quotes for citations.

## Phase 5: On-Site E-E-A-T Enhancements (Your Website Wins Organic & Supports Local)
1. **About page:** Expand with specific "more than three decades," verifiable credentials, personal story (white tiger symbol), trauma-informed/consent language, locations served. Add photo, contact consistency.
2. **Service pages:** One dedicated page per main service (already good structure). Add:
   - What to expect (step-by-step).
   - Session lengths, pricing transparency (where appropriate).
   - Boundaries and what is **not** included.
   - FAQs (already expanding — keep verbatim from your copy).
   - Local context (Manayunk, Northern Liberties, Lambertville NJ).
3. **Schema:** Ensure LocalBusiness + Person (for you) + Service + FAQPage on relevant pages (already adding in PR).
4. **Content:** Publish original, helpful content showing expertise (e.g., "How Breathwork Supports Nervous System Regulation in Philadelphia Clients"). Link internally.
5. **Trust elements:** Prominent phone/email, Calendly, clear "private practice" language, professional boundaries statement on all relevant pages.
6. **Technical:** Fast load, mobile-friendly, HTTPS (already), clear navigation.

**Tip from 2026 factors:** Dedicated service pages + local keywords + NAP on site are top on-page signals.

## Phase 6: Authority & Off-Site Signals
1. Update YouTube channel descriptions, video titles, and about to use current URLs and consistent branding. Add links in descriptions.
2. Amazon author page: Keep updated with latest books; link to current site.
3. Seek media mentions, podcast appearances, or local wellness features (quote in articles, interviews).
4. Build relationships for backlinks: Local Philly wellness sites, complementary practitioners, community orgs.
5. Encourage clients to mention you (with link) on their social if comfortable.
6. Maintain Linktree and socials pointing to current site.

## Phase 7: Monitoring, Measurement & Iteration
1. Google Search Console: Claim property, submit sitemap, monitor coverage (no 404s from old paths), impressions for brand + service terms.
2. Google Analytics / similar: Track traffic from referring sites, time on site, conversions (Calendly clicks).
3. Brand searches: Monitor volume for "Asttarte Deva" vs. old names.
4. Review monitoring tools (e.g., Google alerts, directory alerts).
5. Quarterly audit: Re-check citations, reviews, profile.
6. Track AI Overview appearances for your services (search related queries).

**Success Metrics (3-6 months):**
- Improved local pack visibility.
- More reviews (aim for consistent growth).
- Higher click-through from search.
- Reduced 404 errors in Search Console.
- Stronger "prominence" signals.

## Who Does What
- **Asttarte:** Update external profiles (Yelp, Alignable, about.me, etc.), request reviews, provide copy/photos for site updates, approve content.
- **Kevin / team (us):** Handle repo changes (redirects, schema, pages), technical audits, monitoring setup, commit the plan updates.
- **Both:** Review high-trust referring sites together and decide per-path (update source vs. content page vs. 301).

## Quick Wins (This Week)
1. Claim/optimize GBP.
2. Update 3-5 highest-traffic external listings (start with Yelp, about.me, Alignable).
3. Add 2-3 strong testimonials to the site.
4. Audit one Mailchimp/Wix for outdated links and update if easy.
5. Review the CSV and flag any high-trust paths for no-redirect treatment.

This plan builds on the existing SEO work (FAQs, schema, metas, sitemap) in the PR. Once merged, these actions will compound the technical improvements.

**Next:** Review this with Asttarte, prioritize 3-5 items, and we can implement repo-side changes (e.g., selective redirect adjustments) immediately after merge.

File location: `docs/asttarte-trust-action-plan.md` (committed on branch). Update as progress is made.