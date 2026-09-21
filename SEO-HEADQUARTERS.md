# TravelLingo Website Growth Plan

**Website:** https://gotravellingo.com/  
**Project folder:** `travellingo-landing`  
**Your time:** about **1 hour a day, 5 days a week**  
**Last updated:** 2026-09-21  

## What this file is

This is your **homepage for growing the TravelLingo website**.

Open it at the start of each work session. It tells you:

1. What the goal is  
2. What is already done  
3. What to do next  
4. How to use AI (Cursor) to do most of the writing and checking  
5. What you should personally review before putting anything live  

Update the checklist statuses and the **Work log** at the bottom as you go.

---

## How you and AI work together

You do **not** need to write full articles yourself.

### AI (Cursor) should usually:
- Write new guide pages using the existing Spanish / French / Italian / German pages as a template
- Copy the same look and layout (no redesign)
- Pull German, French, Italian, and Spanish phrases **only** from the TravelLingo app lesson file (`lessons.ts`)
- Update the Guides page, homepage cards, and sitemap when adding a new guide
- Run checks for broken links, missing accents, mobile layout issues, and product wording mistakes
- Suggest next SEO steps based on this plan

### You should usually:
- Decide **what** to work on this week (one main project)
- Provide or approve the hero image for a new guide
- Preview the page locally
- Ask AI to fix anything that looks wrong
- Deploy when you are happy
- Glance at Google Search Console once a week

**Simple rule:** AI builds. You decide, review, and publish.

---

## 1. The big goal

Help more travelers find TravelLingo through Google by publishing useful **travel phrase guides**.

Good guides should:

1. Answer real travel questions (for example: “Italian travel phrases”)
2. Feel helpful first, salesy second
3. Naturally point people to the App Store and Google Play
4. Only show phrases that exist in the TravelLingo app

### Not the goal
- Redesigning the whole website
- Building a big blog empire overnight
- Adding a complicated content system (CMS)
- Chasing every possible keyword

---

## 2. Rules to always follow

### Time rule
Work on **one main project per week**.

Do not start a second big guide until the current one is:

- finished
- linked from the Guides page and homepage (if homepage shows guide cards)
- added to the sitemap
- published (or ready to publish)

### Brand and product rules
- Talk to **travelers preparing for a trip**
- Never say **“beginner travelers”**
- TravelLingo is **not** a full language course
- TravelLingo is **not** mainly a phrasebook
- Do **not** say speaking / speech recognition works offline
- Do **not** say TravelLingo does advanced accent scoring
- Closing brand line (when used):  
  **Travel with confidence. Learn the phrases you’ll actually use.**
- App languages: Spanish, French, Italian, German
- If a phrase is not in `lessons.ts`, do **not** put it on the website

### Website rules
- Keep the current clean TravelLingo design
- New guides should look like the existing language guides
- Put new guides under `/guides/.../`
- Update `sitemap.xml` whenever a new public page goes live
- Do not use “coming soon” or waitlist language on marketing pages

---

## 3. What the site has right now

### Main pages
| Page | What it is | Notes |
|---|---|---|
| Homepage `/` | Main landing page + guide cards | Keep as the front door |
| `/guides/` | List of all travel language guides | Keep this updated |
| Spanish guide | Live language guide | Exists |
| French guide | Live language guide | Exists |
| Italian guide | Language guide | Confirm it is live on the real website |
| German guide | Language guide | Created; confirm it is live |
| Support | Help page | Exists |
| Privacy | Privacy page | Exists |
| `sitemap.xml` | List of pages for Google | Keep updated |
| `robots.txt` | Tells Google it can crawl the site | Exists |

### Good news
You already have a strong start: language guides for Spanish, French, Italian, and German, plus related links between them.

### Still useful next steps
1. Make sure Italian and German are fully live and listed for Google
2. Use Google Search Console every week (even for 10–15 minutes)
3. Later: write situation guides (restaurants, hotels, trains) and destination guides
4. Improve older pages only when Search Console shows a clear problem

---

## 4. What “success” looks like in 90 days

Check these about once a month (not every day):

| What to watch | What “good” looks like | Where to look |
|---|---|---|
| Guide pages found by Google | All published guides show up | Google Search Console → Pages |
| People seeing your pages | Views/impressions go up over time | Search Console → Performance |
| People clicking | Clicks go up over time | Search Console → Performance |
| App downloads from the site | Steady or rising | App store / analytics if you use them |
| Publishing pace | About 1 useful new page every 1–2 weeks | This work log |

**Best strategy right now:** keep the four language guides strong, then add situation pages (like restaurants or hotels) that link back to those language guides.

---

## 5. What to do next (top to bottom)

### Step A — Finish the foundation
- [x] Italian guide in sitemap
- [x] Sitemap submitted in Google Search Console
- [x] robots.txt checked
- [x] Quick mobile check of homepage, Guides page, and one article
- [X ] Confirm Italian is live on gotravellingo.com
- [X ] Confirm German is live on gotravellingo.com
- [X ] Ask Google to index any newly published guides

### Step B — Keep the language set healthy
- [x] German guide created
- [x] German card on Guides page and homepage
- [x] German URL in sitemap
- [x] Related Travel Language Guides links between languages
- [ ] Quick AI check that all related links still work after deploy

### Step C — Improve existing pages (good Thursday tasks)
Ask AI to help with one small item:
- Improve a page title/description only if Search Console shows lots of views but few clicks
- Add or fix one internal link
- Compress a large image if a page feels slow
- Re-check mobile layout on one guide
- Optional cleanup: change Support and Privacy links from `/support.html` and `/privacy.html` to `/support` and `/privacy` (the `.html` links already work via redirect; this just skips the extra hop)

### Step D — New content ideas (after foundation is solid)
Do **one** at a time. Ask AI to write it using the current guide template.

**Situation guides**
- Restaurant and café phrases
- Hotel phrases
- Directions phrases
- Transportation phrases
- Emergency / health phrases (be careful and accurate)

**Destination guides** (later)
- Example: useful Spanish for a Mexico trip
- Needs a real photo and careful wording
- Still only use phrases from the app

**Helpful explainer pages**
- How to practice travel phrases before a trip
- Travel phrases vs a full language course

### Step E — Later / maybe never
- Big redesign
- CMS
- Newsletter
- Lots of thin AI blog posts with no real value

---

## 6. How to make a new guide with AI

A full new guide usually takes about **2–4 of your hours**, because AI does the heavy writing.

### Day 1 — Decide and gather (about 30–60 minutes)
1. Choose the next guide from the backlog below
2. Make sure you have (or can get) one good royalty-free photo
3. Put the photo in `public/assets/` if needed
4. Open Cursor and paste a clear request (see section 11)

### Day 2 — Let AI build (about 30–60 minutes)
Ask AI to:
1. Copy the structure of an existing language guide
2. Write the new page
3. Use only phrases from `lessons.ts`
4. Update the Guides page, homepage cards, and sitemap
5. Run a check list (links, accents, mobile, brand rules)

### Day 3 — You review (about 30–60 minutes)
Look at the page yourself and ask:
- Does it look like the other guides?
- Are accents / special letters correct?
- Do the store badges work?
- Does it feel helpful, not spammy?
- Did AI invent any phrases? (If unsure, ask AI to re-check against `lessons.ts`)

### Day 4 — Publish and confirm (about 15–30 minutes)
1. Deploy using your normal process
2. Open the live URL on your phone
3. In Search Console, ask Google to index the new page if needed
4. Mark the backlog item Done
5. Write a short note in the Work log

---

## 7. Link rules (keep it simple)

Every new guide should be linked from:

1. The Guides page (`/guides/`)
2. The homepage guide cards (if that section exists)
3. The sitemap
4. The Related Travel Language Guides section on other language guides (when it makes sense)

Every guide should also link back to:

- `/guides/`
- App Store and Google Play badges (already on the pages)

Never link to a page that is not published yet.

---

## 8. Backlog (your to-do list)

Statuses you can use: `Queued` / `In progress` / `Done` / `Blocked`

| # | Project | Status | Notes |
|---|---|---|---|
| 1 | Confirm Italian is live + indexed | Queued | Open live URL; check Search Console |
| 2 | Confirm German is live + indexed | Queued | Open live URL; check Search Console |
| 3 | Related links across Spanish/French/Italian/German | Done | Already added |
| 4 | First situation guide (restaurants) | Queued | Ask AI to write after language set is live |
| 5 | Hotel phrases guide | Queued | |
| 6 | Getting-around phrases guide | Queued | |
| 7 | “How to prepare travel phrases before a trip” | Queued | Good brand-supporting page |
| 8 | First destination guide | Queued | Needs photo + careful wording |
| 9 | Title/description improvements based on Search Console | Queued | Wait until you have a few weeks of data |
| 10 | Light support/privacy SEO cleanup | Queued | Only if Google shows problems |
| 11 | Optional: update Support/Privacy links to `/support` and `/privacy` | Queued | Not urgent. Live `.html` links already redirect successfully; cleanup only removes the redirect hop |

---

## 9. Weekly schedule (about 5 hours total)

### Monday — Pick one thing
- Open this file
- Choose **one** backlog item
- Ask AI to start it, or review what AI already made

### Tuesday — Continue
- Keep working on the same item only
- Ask AI for fixes if something looks off

### Wednesday — Finish and prepare to publish
- Finish the page
- Ask AI to run final checks
- Preview on desktop and phone

### Thursday — Check and maintain
Pick one small task:
- Look at Search Console
- Ask AI to check for broken links
- Fix one small issue
- Improve one weak title only if data supports it

### Friday — Wrap up
- UpdateStatuses in this file
- Write next week’s one priority in the Work log
- Stop. Do not start a brand-new big project late on Friday

### Once a month
Replace Thursday with a bigger review:
- Which pages got the most views?
- Which pages got clicks?
- Should next month focus on a new page, or improving an old one?

---

## 10. Google Search Console (in plain English)

Google Search Console is a free Google tool that shows:

- whether Google found your pages
- which searches show your site
- how often people click

### Set up once
- [ ] Add `gotravellingo.com` in Google Search Console
- [ ] Submit sitemap: `https://gotravellingo.com/sitemap.xml`
- [ ] Confirm the site uses https

### Check weekly (10–20 minutes)
Ask yourself:
1. Did any new page have errors?
2. Which guide got the most views?
3. Which guide got clicks?
4. Is there an obvious broken page to fix?

### Important patience rule
After publishing a new page, wait **about 4–8 weeks** before rewriting it just for SEO.

---

## 11. Ready-to-paste AI request

When you want Cursor to create the next guide, paste something like this:

> Please create the next TravelLingo guide.  
> Use the existing Spanish, French, Italian, and German guides as the exact visual and structural template.  
> Do not redesign the site.  
> Only use phrases that exist in the TravelLingo app lesson file (`lessons.ts`).  
> Update `/guides/`, the homepage guide cards if present, and `sitemap.xml`.  
> Add or update Related Travel Language Guides links only to published pages.  
> Then run checks for: one H1, accents/special characters, mobile overflow, store badges, brand wording rules, and broken internal links.  
> Follow `SEO-HEADQUARTERS.md`.  
> Do not commit, push, or deploy unless I ask.

When you want AI to check the site:

> Please review the TravelLingo website against `SEO-HEADQUARTERS.md`.  
> Check published guides for broken links, missing related links, product wording mistakes (offline speech recognition, beginner travelers, fluency claims), and mobile layout issues.  
> Report problems first. Do not change files until I approve.

---

## 12. Topics that fit TravelLingo

### Strong topics you already own
- Spanish travel phrases
- French travel phrases
- Italian travel phrases
- German travel phrases

### Good next topics
- Restaurant phrases for [language]
- Hotel phrases for [language]
- Directions / transportation phrases
- How to practice travel phrases before a trip

### Avoid for now
- Generic “become fluent” pages
- Thin AI pages with no real travel value
- Keyword-stuffed titles that sound unnatural
- Claims the app cannot support

---

## 13. Quick check list before publishing

Ask AI to verify these, then spot-check yourself:

- [ ] Page title and short description make sense
- [ ] Canonical URL is correct
- [ ] Exactly one main title (H1)
- [ ] Headings are in a sensible order
- [ ] All phrases exist in the app lesson file
- [ ] Accents / umlauts / special characters look right
- [ ] Hero image loads
- [ ] Page looks okay on a phone
- [ ] Guides page card exists
- [ ] Homepage card exists (if homepage shows cards)
- [ ] Sitemap includes the new URL
- [ ] Related links only go to published pages
- [ ] App Store and Google Play badges still work
- [ ] No offline speech-recognition claims
- [ ] No “beginner travelers” wording

---

## 14. If you get stuck

| Situation | What to do |
|---|---|
| You have less than 45 minutes | Ask AI for a small check or fix. Do not start a whole new guide. |
| A guide is almost done | Finish and publish it before starting anything else. |
| You are unsure about a phrase | Ask AI to check `lessons.ts`. If it is missing, leave it out. |
| You feel tempted to redesign | Stop. Improve content and links instead. |
| A page gets views but few clicks | Ask AI to suggest a clearer title and description. |
| You want faster growth | Publish the next useful guide. Do not rebuild the whole site. |

---

## 15. Work log

Write one line after each work session.

| Date | Minutes | What I did | Next action |
|---|---|---|---|
| 2026-09-21 | — | Growth plan rewritten for AI-first workflow | Confirm Italian + German are live |
|  |  |  |  |
|  |  |  |  |

---

## 16. Suggested plan for this week

**Week goal:** Confirm Italian and German are live, then choose the first situation guide.

| Day | What to do |
|---|---|
| Mon | Open live Italian and German URLs; confirm they work on phone |
| Tue | In Search Console, check whether Google sees the new guides |
| Wed | Ask AI to propose the best next situation guide and draft an outline |
| Thu | Approve the outline; ask AI to write the first draft if ready |
| Fri | Update this backlog and pick next week’s one priority |

---

## Plain-English glossary

| Term | Meaning |
|---|---|
| SEO | Helping your site show up in Google search results |
| Guide | A helpful article page on your website |
| Sitemap | A file that lists your public pages for Google |
| Indexing | Google finding and storing a page so it can appear in search |
| Search Console | Google’s free dashboard for site search performance |
| Canonical URL | The official web address for a page |
| Internal link | A link from one of your pages to another of your pages |
| CTR | Click-through rate: how often people click after seeing your page in Google |
| Deploy | Putting your local website changes onto the live website |

---

Keep this file simple.  
When something is finished, mark it Done and move on.  
Let AI do the writing and checking. You stay in charge of priorities, review, and publishing.
