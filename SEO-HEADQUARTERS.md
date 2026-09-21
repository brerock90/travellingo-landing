# TravelLingo Website SEO Headquarters

**Site:** https://gotravellingo.com/  
**Repo:** `travellingo-landing` (static site on Cloudflare Pages)  
**Your capacity:** ~1 hour/day × 5 days/week ≈ **5 hours/week**  
**Last updated:** 2026-09-21  

Use this file as the single source of truth for what to work on next. Open it at the start of each work session. Update the **Status** column and the **Log** at the bottom when you finish something.

---

## 1. Mission (keep this short)

Grow organic discovery for TravelLingo by publishing **practical travel-phrase guides** that:

1. Rank for destination / language intent (“Italian travel phrases”, etc.)
2. Naturally send readers to the App Store / Google Play
3. Stay accurate to the app (phrases only from `lessons.ts`)

**Not the mission:** build a media company, chase every keyword, redesign the brand, or ship a CMS.

---

## 2. Constraints (do not violate)

### Time
| Block | Minutes | Typical use |
|---|---|---|
| Mon | 60 | One unfinished content task OR technical SEO |
| Tue | 60 | Continue same content task |
| Wed | 60 | Finish + ship + sitemap/internal links |
| Thu | 60 | Measurement / refresh / small wins |
| Fri | 60 | Plan next week + backlog grooming |

Rule: **one primary project per week.** Do not start a second guide until the current one is live and linked.

### Product / brand accuracy
- Audience: travelers preparing for a trip — **never** “beginner travelers”
- TravelLingo is **not** a fluency course and **not** primarily a phrasebook
- Speech recognition **requires connectivity** — never imply offline speaking practice
- No advanced accent-scoring claims
- Official tagline only when closing branded CTAs:  
  *Travel with confidence. Learn the phrases you’ll actually use.*
- Languages in app: Spanish, French, Italian, German
- Italian/French/Spanish guide phrases must exist in app `lessons.ts` before publishing

### Site architecture (keep it)
- Static HTML under `public/`
- Guides at `/guides/<slug>/`
- Reuse Spanish/French/Italian guide HTML/CSS patterns — no redesign
- Root-relative asset paths (`/styles.css`, `/assets/...`)
- Update `sitemap.xml` when a new public URL goes live
- No waitlist / “coming soon” language on marketing pages

---

## 3. Current baseline (as of 2026-09-21)

### Live / ready pages
| URL | Role | Status |
|---|---|---|
| `/` | Homepage + guide preview cards | Live pattern |
| `/guides/` | Guide index | Live |
| `/guides/spanish-for-travel/` | Spanish pillar | Live |
| `/guides/travel-phrases-in-french/` | French companion | Live |
| `/guides/travel-phrases-in-italian/` | Italian companion | Local / ship when ready |
| `/support.html` | Support | Live |
| `/privacy.html` | Privacy | Live |
| `/sitemap.xml` | Sitemap | Present |
| `/robots.txt` | Crawl rules | Present |

### Gaps (high leverage)
1. **German language guide** missing (completes the 4-language set)
2. **Search Console** setup / monitoring not yet a weekly habit
3. No **destination-focused** guides yet (high intent, later phase)
4. No systematic **internal linking** between language guides
5. Homepage / guides index may need copy refresh after German ships
6. Italian page must be confirmed deployed + indexed

---

## 4. North-star outcomes (90 days)

Track these monthly — not daily.

| Metric | Target direction | Where to look |
|---|---|---|
| Indexed guide pages | All published guides indexed | Google Search Console → Pages |
| Non-brand impressions | Up month over month | GSC → Performance |
| Clicks to guides | Up month over month | GSC → Performance |
| App store referrals from site | Stable or up | Analytics / store campaign if used |
| Guide completion rate | Finish 1 substantial content unit / 1–2 weeks | This HQ log |

**Primary SEO bet:** finish the **language-phrase guide cluster** (ES / FR / IT / DE), then expand into **destination** and **situation** pages that link back into that cluster.

---

## 5. Priority ladder (work top → bottom)

### P0 — Foundation (do first if incomplete)
- [ ] Confirm Italian guide deployed and in `sitemap.xml`
- [ ] Submit / resubmit sitemap in Google Search Console
- [ ] Verify `robots.txt` allows crawling and points at sitemap
- [ ] Spot-check mobile: homepage, `/guides/`, one article

### P1 — Finish language cluster (next 2–4 weeks)
- [ ] German guide: `/guides/travel-phrases-in-german/` (mirror FR/IT structure)
- [ ] Add German card to `/guides/` and homepage preview
- [ ] Add German URL to `sitemap.xml`
- [ ] Cross-link language guides (see §7)

### P2 — Strengthen existing pages (ongoing Thursdays)
- [ ] Refresh thin sections if GSC shows impressions but low CTR
- [ ] Improve titles/meta only when CTR data justifies it
- [ ] Add 1–2 natural internal links per older guide when new guides ship
- [ ] Compress oversized guide images only if load feels slow

### P3 — Expand topics (after German is live)
Ship **one** of these at a time:

**Situation pages** (reuse phrase categories from the app)
- Restaurants & cafés phrases (language-specific or multi-language hub)
- Hotel check-in phrases
- Asking for directions
- Transportation phrases
- Emergency / health phrases (careful, accurate)

**Destination pages** (later; need real photos + careful claims)
- e.g. “Useful Spanish for Mexico travel” / “French for Paris trip”
- Only after language pillars exist
- Must not invent phrases outside the app

**Comparison / intent pages** (careful; avoid fluff)
- Travel phrases vs full language course
- How to practice travel phrases before a trip

### P4 — Do later / only if capacity
- Blog cadence beyond guides
- Email / newsletter
- Localized site versions
- CMS
- Heavy redesign
- Affiliate content

---

## 6. Content production playbook (one guide ≈ 3–5 hours)

Use this checklist for every new guide. Copy it into the weekly log when you start.

### Session A (≈60–90 min) — Research & outline
1. Open app lesson source: `lessons.ts` for that language
2. List phrases by category you will include (greetings, food, directions, transport, hotel, shopping, misunderstanding, emergency)
3. Reject any phrase not in the app
4. Draft H1, meta title, meta description, URL slug
5. Confirm or source one royalty-free hero image into `public/assets/`

### Session B (≈60–90 min) — Write body
1. Duplicate the French or Italian guide HTML as the template
2. Replace metadata, breadcrumbs, hero, phrases, copy
3. Keep structure identical (hero → intro → H2 sections → CTA)
4. Preserve store badge URLs and tagline

### Session C (≈45–60 min) — Integrate & QA
1. Add card on `/guides/index.html`
2. Add card on homepage guide section
3. Add URL to `sitemap.xml`
4. Local preview: accents, mobile overflow, one H1, badges
5. Deploy when ready (your process — not automatic from this HQ)

### After publish (≈15–30 min next day)
1. Request indexing in Search Console (if available)
2. Click through live URLs
3. Mark status Done in §8 backlog
4. Add 1 internal link from an older related guide

**Estimated cadence at 5 hrs/week:** ~1 full language guide every **1–2 weeks**, or 1 smaller refresh week between guides.

---

## 7. Internal linking rules

Minimum links for every new guide:
- Homepage preview card → guide
- `/guides/` card → guide
- Guide → `/guides/`
- Guide CTA → App Store + Google Play (existing badges)

When 3+ language guides exist, add a short “Related Travel Language Guides” note near the end of each article linking to the other languages — **only** to published pages.

Do not link to unpublished URLs.

---

## 8. Content backlog (ordered)

Update status: `Queued` / `In progress` / `Done` / `Blocked`

| # | Asset | Suggested slug | Est. hours | Status | Notes |
|---|---|---|---|---|---|
| 1 | Confirm Italian live + indexed | `/guides/travel-phrases-in-italian/` | 0.5 | Queued | Verify deploy + GSC |
| 2 | German travel phrases guide | `/guides/travel-phrases-in-german/` | 4–5 | Queued | Mirror FR/IT; phrases from `lessons.ts` |
| 3 | Cross-links across ES/FR/IT/DE | n/a | 1 | Queued | After German ships |
| 4 | Title/meta CTR pass on top guides | n/a | 1–2 | Queued | After 4–6 weeks of GSC data |
| 5 | Situation: restaurants (start with one language) | TBD | 3–4 | Queued | After language cluster |
| 6 | Situation: hotels | TBD | 3–4 | Queued | |
| 7 | Situation: getting around | TBD | 3–4 | Queued | |
| 8 | Destination highlight #1 | TBD | 4–5 | Queued | Needs photo + careful regional copy |
| 9 | “How to prepare travel phrases before a trip” | TBD | 2–3 | Queued | Supports brand positioning |
| 10 | Privacy/support SEO light pass | existing pages | 1 | Queued | Only if crawl/index issues |

---

## 9. Weekly operating rhythm

### Monday — Choose & start
- Read this HQ (§5–§8)
- Pick **one** backlog item
- Work 50 minutes; leave a 10-minute note in the Log

### Tuesday / Wednesday — Build
- Continue the same item only
- Ship by end of Wednesday if possible

### Thursday — Measure & maintain
Pick **one**:
- Search Console: queries, pages, coverage
- Fix a broken link / mobile issue
- Add one internal link
- Improve one underperforming title (only with data)

### Friday — Close the loop
- Update backlog statuses
- Write next week’s single priority in the Log
- Stop. Do not start a new big project Friday afternoon

### Monthly (first Thursday of month, replace normal Thursday)
- Review impressions/clicks by page
- Decide: new content vs refresh existing
- Archive ideas that don’t fit product accuracy rules

---

## 10. Measurement setup checklist

Do once, then check weekly on Thursdays.

- [ ] Google Search Console property for `gotravellingo.com`
- [ ] Sitemap submitted: `https://gotravellingo.com/sitemap.xml`
- [ ] Preferred domain / HTTPS confirmed
- [ ] Optional: privacy-friendly analytics (only if you want referral paths)
- [ ] Spreadsheet or note for monthly snapshot:  
  `Date | Clicks | Impressions | CTR | Top page | Top query`

Do **not** optimize titles weekly without data. Give new pages **4–8 weeks** before major rewrites.

---

## 11. Keyword / topic map (working)

Focus on **intent match**, not volume chasing.

### Language pillars (owned)
- Spanish for travel / Spanish travel phrases
- French travel phrases / practical French for travelers
- Italian travel phrases / practical Italian for travelers
- German travel phrases / practical German for travelers ← next

### Supporting intents (later)
- [language] restaurant phrases
- [language] hotel phrases
- [language] directions / transportation
- travel phrases before a trip
- how to practice travel language offline-safe claims only where true (audio/reference ≠ speech recognition)

### Avoid for now
- Generic “learn Italian online” fluency SERPs
- Phrasebook dump pages with no narrative
- Thin AI-spun destination posts with no unique value
- Keyword-stuffed titles that break brand voice

---

## 12. Technical SEO checklist (static site)

Run when shipping pages or monthly.

- [ ] Unique `<title>` and meta description per page
- [ ] Canonical matches live URL
- [ ] One H1; logical H2/H3
- [ ] `sitemap.xml` includes only live public URLs
- [ ] `robots.txt` allows `/` and lists sitemap
- [ ] Images: descriptive alt, controlled crop via existing CSS, lazy-load cards only
- [ ] No orphan pages (every new guide linked from `/guides/` + ideally homepage)
- [ ] Fast enough on mobile (avoid huge unoptimized heroes when possible)
- [ ] Store badge links unchanged and working

---

## 13. Agent / Cursor brief (paste when requesting help)

When asking Cursor to build the next guide, paste:

> Create the next TravelLingo guide using `/guides/travel-phrases-in-french/` and `/guides/travel-phrases-in-italian/` as the structural template. Do not redesign. Pull phrases only from `lessons.ts`. Update `/guides/`, homepage cards if present, and `sitemap.xml`. Do not commit/push/deploy unless I ask. Follow product accuracy rules in `SEO-HEADQUARTERS.md`.

---

## 14. Decision rules (when stuck)

| Situation | Decision |
|---|---|
| Less than 45 minutes today | Do measurement or a 1-link internal-link task — do not start a new guide |
| Guide 80% done | Finish and ship before starting anything else |
| Unsure if a phrase is allowed | Check `lessons.ts` — if absent, omit it |
| Tempted to redesign | No — improve content and linking instead |
| Page got impressions, low CTR | Test a clearer title/meta; keep H1 aligned |
| Page got clicks, high bounce | Improve intro + early phrase usefulness; check mobile |
| Want more traffic fast | Ship German guide; then situation pages — not ads-heavy redesign |

---

## 15. Work log

Add a line after each work session.

| Date | Minutes | What I did | Next action |
|---|---|---|---|
| 2026-09-21 | — | HQ file created | Confirm Italian deploy + start German research |
|  |  |  |  |
|  |  |  |  |

---

## 16. One-week starter plan (copy into Log)

**Week goal:** Italian confirmed live + German guide Session A complete.

| Day | Task |
|---|---|
| Mon | Deploy/verify Italian; GSC sitemap check (60 min) |
| Tue | German: extract phrases from `lessons.ts` + outline sections (60 min) |
| Wed | German: find/confirm hero image + draft metadata/slug (60 min) |
| Thu | GSC review + add any missing internal links on FR/IT (60 min) |
| Fri | Update this HQ backlog statuses; lock next week = German draft HTML (30–60 min) |

---

*End of headquarters. Keep this file lean — move finished detail into git commits and leave only current priorities here.*
