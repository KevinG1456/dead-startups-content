# YouTube Production Pipeline — Step-by-Step Guide

**Channel niche:** Forensic documentaries on funded software companies that died — reconstructed from
their own metrics, pitch decks, Crunchbase trails, shutdown letters, and post-mortems.
**Audience:** Founders, indie hackers, PMs, VCs/angels, startup employees, B2B sales/marketing —
global, English-first, high-income, professional software buyers.

**The pipeline, in one line:**

```
TITLE → Claude Code (research + package) → ChatGPT (thumbnail) → HeyGen Avatar V (presenter video)
      → Video Editor (final cut) → YouTube (upload + distribute)
```

| Stage | Owner | Output |
|---|---|---|
| 🧠 Brain | Claude Code | Full 18-file research + content package |
| 🎨 Thumbnail/Creative Director | ChatGPT | Final thumbnail image(s) |
| 🎥 Presenter | HeyGen Avatar V | Avatar-narrated video segments |
| 🎬 Final production | Video editor | Assembled, graded, scored final video |
| 📺 Distribution | YouTube + cross-platform | Published video, Shorts, posts, email |

This document walks through every stage in order, from picking a topic to publishing and promoting
the finished video. It reflects how this channel **actually** operates today (verified against 40
built packages), not just the aspirational spec — where the two differ, that's called out explicitly.

---

## Step 0 — Pick a Topic

New titles come from one of three sources, in order of preference:

1. **A previously-flagged real candidate.** Check `project_factcheck_status.md` (memory) and each
   existing package's own `sources-log.txt` for companies that came up during research but weren't
   used — e.g. comparators mentioned in passing, or companies set aside because they didn't fit that
   package's specific angle. This is the cheapest, most reliable source of new topics.
2. **A batch idea-list file**, e.g. `dead-saas-30-Content Titles new-video-ideas/...md` or the
   `Content Titles V2/V2f/V3/V4.txt` files. These are **pattern-first hypotheses**, not confirmed
   facts — a title like "the startup that got margin-called" describes a *shape* of story, not a real,
   named company. It must survive a real sourcing pass before it's treated as viable (see Step 1a).
3. **Cold research** — picking a real company with no prior lead and researching it from scratch. This
   is an established, workable option (see packages 024, 031+), used when the first two sources are
   exhausted or don't fit what's needed next.

**Do not skip the sourcing check to save time.** Roughly a third of the pattern-first titles tried in
this channel's history turned out to have no real, publicly-documented company behind them at all
(see Step 1a) — finding that out *before* committing to a full build is the entire point of Step 0.

---

## Step 1 — Research & Package Generation (Claude Code) 🧠

This is the foundation everything downstream depends on. Nothing moves to ChatGPT or HeyGen until this
step is fully done and the package passes its own quality gates.

### 1a. Verify the topic is real before building anything

For a pattern-first title (Source #2 above), research a real anchor company first:
- Does a real, named company match this exact pattern?
- Is it independently corroborated across multiple credible sources (not just one blog/aggregator)?
- Is it distinct from every company already used elsewhere on this channel? (Grep
  `YouTube-Content/` for the candidate company's name before committing.)

**If no real anchor survives this check, skip the title.** Log the reasoning in memory
(`project_channel_overview.md`) and move to the next one. Forcing a fabricated or unverifiable example
onto a real company's name — or worse, inventing a plausible-sounding company that doesn't exist —
breaks this channel's core credibility. This has happened: search-engine synthesis sometimes produces
a specific-sounding example (a company name, a funding figure, a "shut down in [month]" detail) that
turns out to trace back to a single low-credibility source or nothing at all. Always independently
verify any single-sourced "real example" before using it — see Step 1c.

### 1b. Confirm the folder and title

Once a real anchor is confirmed:
- Next package number = highest existing `YouTube-Content/0NN-*` folder + 1.
- Folder name format: `0NN-Slug-Name-With-Hyphens` (see any existing package for the pattern).
- The working title can — and often should — diverge from a batch doc's literal wording once real
  numbers are known. If the source doc says "$200M offer, $0 outcome" and the real figures are $30M
  and a $39M sale, **use the real numbers**, not the doc's placeholder framing. State this correction
  explicitly in the package's README and sources-log.

### 1c. Research and source every factual claim

- Prioritize primary sources: SEC/EDGAR filings, court/bankruptcy records, company blog posts, direct
  quotes from named executives, litigation releases from regulators (SEC, DOJ).
- Secondary sources (TechCrunch, Bloomberg, CNBC, Reuters, trade press) are fine for corroboration but
  should be cross-checked against at least one other independent outlet for load-bearing figures.
- **Verify anything that appears in only one low-credibility source before using it.** If a claim
  (a company name, a specific dollar figure, a specific date) can't be independently corroborated,
  either drop it or flag it explicitly as `[VERIFY]`/unconfirmed in the package — never present it as
  settled fact.
- **Handle sensitive claims with extra care.** Serious, unproven allegations against real, living,
  non-convicted people (lawsuits alleging personal misconduct, fraud allegations, etc.) should either
  be deliberately excluded if tangential to the actual story (document that decision in the sources-log
  with reasoning), or handled with the same rigor as a legal/investigative piece: attributed precisely,
  never stated as fact, and reviewed for whether it's actually necessary to the story being told.
- **Political/legal events involving real government action** (pardons, commutations, indictments)
  get stated with strict who/what/when neutrality — zero motive speculation, zero political framing —
  in every file that touches them, including Shorts and social posts.
- If a package's premise doesn't survive the sourcing pass (the batch doc's claim turns out to be
  wrong, exaggerated, or only partially true), **correct it and say so plainly** in the README and
  sources-log rather than silently forcing the content to fit the original framing. This channel has
  done this repeatedly and it's a feature, not a failure.

### 1d. Generate the full 18-file package

Every package folder gets exactly these 18 files (this is the **current, actual** structure — see the
note on the legacy MASTER/language structure at the end of this section):

| File | Purpose | Used at pipeline stage |
|---|---|---|
| `README.md` | Package status, the real case summary, framing requirements, title analysis, viewer psychology, competitor analysis, performance prediction, improvement suggestions | Pre-production review (Step 2) |
| `sources-log.txt` | Full citation map, `[VERIFY]` flags, "BEFORE RECORDING" checklist, editorial decisions and why | **Read in full before every other step** |
| `titles.md` | 20 viral + 10 SEO + 10 curiosity + 10 emotional + 10 high-CTR titles, ranked, with a recommended final title | Pre-production (Step 2) |
| `thumbnails.md` | 3 thumbnail concepts (A/B/C) with full visual spec each, A/B testing table | Thumbnail stage (Step 3) |
| `ai-image-prompts.md` | Ready-to-paste image-generation prompts (thumbnail, backgrounds, illustrations, infographics, scene art) | Thumbnail stage (Step 3) |
| `script.md` | 20 hooks, full production script with cold open/hooks/segments/CTAs, 3 alternate script versions, retention notes, chapters | Video production (Step 4) |
| `heygen-production.md` | Avatar performance direction + full scene-by-scene breakdown mapped to the script | Video production (Step 4) |
| `editing-notes.md` | Zoom/motion graphics/lower thirds/animations/camera/music/SFX, beat by beat | Editing (Step 5) |
| `seo.md` | Primary/secondary/long-tail/semantic/trending keywords, related searches | Metadata (Step 6) |
| `description.md` | SEO, story, long, and short description variants with chapters | Metadata (Step 6) |
| `tags.md` | 100 tags (primary/secondary/long-tail/trending/competitor) | Metadata (Step 6) |
| `hashtags.md` | 30 hashtags | Metadata (Step 6) |
| `publishing-plan.md` | Best time, target audience, playlist, end screen, cards, end CTA | Publishing (Step 7) |
| `shorts.md` | 10 Shorts ideas, each with hook/script/CTA | Shorts (Step 8) |
| `community-posts.md` | 5 pinned-comment versions + 10 community posts | Cross-promotion (Step 9) |
| `social-posts.md` | Platform-specific copy for X, Threads, LinkedIn, Facebook, Instagram, TikTok, Bluesky | Cross-promotion (Step 9) |
| `email-campaign.md` | Launch, reminder, and final-chance emails | Cross-promotion (Step 9) |
| `blog.md` | Full SEO blog article version of the script + 30-question FAQ | Cross-promotion (Step 9) |

**Note on the MASTER/language-folder structure:** packages 001–004 were built with a `MASTER/` folder
plus per-language subfolders (`EN/`, `DE/`, `FR/`, `NL/`, `NO/`, `SV/`), per the original 6-language
localization plan. That structure was never finished for those packages (only 004 and 009 have partial
language folders) and packages 005 onward all use the flat 18-file structure above, English-only, as
the actual default. **Treat the flat, English-only structure as the current standard** for every new
package. Localization is still a live, intended initiative — see Step 10 for how to resume it, but
don't block a new package's production on it.

### 1e. Fact-check gate — do not proceed until this passes

Before moving to Step 2:
- [ ] Every named company, person, date, and dollar figure in the package traces to a source in
      `sources-log.txt`.
- [ ] Every `[VERIFY]` item is flagged consistently across all 18 files where it appears (not stated
      as fact in one file and flagged in another).
- [ ] The "BEFORE RECORDING" checklist in `sources-log.txt` is complete and specific.
- [ ] No file conflates this company with a similarly-named or easily-confused one (check this
      explicitly if the story involves two related entities, e.g. two products by the same team, or
      two companies with similar names).
- [ ] Update `project_factcheck_status.md` (memory) with a summary entry for the new package,
      including any pivots made during research.

---

## Step 2 — Pre-Production Review

Before generating any images or video, whoever is producing the video should:

1. Read `README.md` in full — confirms the real case and any framing requirements.
2. Read `sources-log.txt` in full, especially the "BEFORE RECORDING" section — this is the single most
   important file in the package for avoiding an on-camera factual error.
3. Confirm the final title from `titles.md`'s "Recommended Title" (or pick a strong alternate from the
   ranked list if a different angle is preferred for this specific upload).
4. Note any sensitivity flags (excluded content, neutrality requirements, "never state X as fact")
   that must be respected in every downstream asset — thumbnail text, Short scripts, social posts, all
   of it.

---

## Step 3 — Thumbnail Creative Direction (ChatGPT) 🎨

**Golden rule: the strongest thumbnails communicate one dominant idea instantly.** Never try to
illustrate the whole video in one image.

1. Open `thumbnails.md` and pick the primary concept (usually "Version A," the recommended/highest-CTR
   option) plus one or two alternates for A/B testing.
2. Feed the corresponding prompt(s) from `ai-image-prompts.md` directly to ChatGPT (or Midjourney/Flux/
   Ideogram — the prompts are written to be compatible with all of them).
3. **Never render a real, identifiable photorealistic likeness of a real named person** in a generated
   thumbnail — every package's `ai-image-prompts.md` and `thumbnails.md` already builds this in as a
   standing rule. If a real person's face is wanted, use licensed/rights-cleared photography added in
   the editor, not an AI generation.
4. **Never render real company logos, wordmarks, or trademarked iconography** in a generated image —
   same rule. Add verified real branding in the editor afterward if needed, with proper rights
   clearance.
5. Generate 2–4 variations of the winning concept, pick the strongest, and keep at least one A/B
   alternate on hand for the "A/B Testing" table in `thumbnails.md`.
6. **The thumbnail, the title, and the first 30 seconds of the video need to tell the same story.**
   Once the thumbnail is locked, make sure the cold open in `script.md` still matches its promise —
   adjust the cold open if the chosen thumbnail leads with a different angle than the script currently
   opens with.

---

## Step 4 — Video Production (HeyGen Avatar V) 🎥

1. Open `heygen-production.md` — this is a complete, ready-to-use scene-by-scene blueprint: avatar
   model, presenter performance direction (energy, pace, tone, expression, gestures), and a full
   scene list with duration, avatar-vs-B-roll split, script text, and visual direction for each beat.
2. Feed each scene's script text into HeyGen with Avatar V as the primary model. (Avatar IV is the
   secondary option — reach for it only for special characters, more experimental visual storytelling,
   or when more custom prompting control is needed than Avatar V's consistency-focused mode allows.)
3. **Do not make the entire video an avatar talking to camera.** Follow the alternating pattern the
   scene breakdown already encodes:
   - 0:00–0:20 — Avatar V, strong hook, pattern interrupt, presenter on screen
   - 0:20–1:00 — B-roll + narration (AI visuals, screenshots, charts, text animations)
   - 1:00–1:30 — Avatar V, introduce the next major point
   - 1:30–3:00 — B-roll / graphics / narration
   - 3:00–3:20 — Avatar V, emotional/curiosity beat
   - ...continue this alternating rhythm for the full runtime.
4. Export each scene's raw avatar footage, keeping the scene numbering from `heygen-production.md`
   intact so the editor (Step 5) can match footage to editing notes without re-deriving the mapping.

---

## Step 5 — Editing (Video Editor) 🎬

1. Open `editing-notes.md` — organized by the same segments as `script.md`, covering zoom suggestions,
   motion graphics (with exact on-screen text for every title card), lower thirds (including standing
   attribution/caveat tags that must appear whenever specific claims are on screen), animations, camera
   movement, background music direction per segment, and sound effects per beat.
3. Assemble avatar footage (Step 4) with B-roll, motion graphics, and title cards exactly as specified
   — the editing notes are written to be followed literally, including *when a framing/caveat card must
   be held on screen for a full beat rather than flashed quickly* (this matters most in segments dealing
   with `[VERIFY]` items, sensitive claims, or founder-distinction framing).
2. Pull chapter timestamps directly from the "Chapters / Timestamps" section at the bottom of
   `script.md` — use these for both the YouTube chapters field (Step 6) and any on-screen chapter
   markers.
4. Never fabricate or reconstruct a real company's actual product UI, internal documents, or specific
   branded assets in motion graphics — use generic, unbranded representations as instructed, and add
   real screenshots/footage only where rights-cleared source material exists.
5. Final pass: confirm every on-screen text card matches the exact wording and framing specified in
   `editing-notes.md` and `script.md` — this is the last checkpoint before a fact-check error could
   make it into the published video.

---

## Step 6 — Metadata & SEO

When creating the YouTube upload:

1. **Title:** the recommended title from `titles.md` (or the A/B alternate chosen for this specific
   test).
2. **Description:** use the "SEO Description (default)" from `description.md` for the primary upload;
   the "Long Description," "Story Description," and "Short Description" variants are available for
   A/B testing or for repurposing on other platforms (blog, email). Paste the chapters block from
   `description.md` directly into the description — it's pre-formatted for YouTube's chapter parser.
3. **Tags:** paste all 100 tags from `tags.md` into YouTube's tag field (YouTube truncates around
   500 characters total — prioritize Primary and Secondary tags first if space runs out).
4. **Hashtags:** the 30 hashtags in `hashtags.md` — YouTube only displays the first 3 above the title,
   so make sure the 3 most important ones lead the description's hashtag line.
5. Double-check the description and pinned comment don't contradict any `[VERIFY]` or exclusion flag
   from `sources-log.txt`.

---

## Step 7 — Publishing

1. Open `publishing-plan.md` for: best publishing day/time, target audience framing, which playlist(s)
   to add the video to, end-screen video pairing, in-video cards (with exact timestamp placement), and
   the scripted end CTA.
2. Schedule the upload for the recommended window (this channel's default: Tuesday–Thursday,
   9–11am ET, unless a package's `publishing-plan.md` calls for something different due to news-cycle
   timing or recency).
3. Add the video to every playlist named in `publishing-plan.md`, including any cross-reference
   playlists connecting it to related packages (e.g. a shared "cap-table mechanics" or "SPAC casualties"
   playlist).
4. Set the end screen and cards exactly as specified — many packages deliberately avoid pairing with a
   thematically-similar-but-tonally-wrong package (e.g. never end-screen a non-fraud package next to a
   real-conviction fraud package just because both involve "criminal charges").
5. Post the pinned comment (one of the 5 versions in `community-posts.md`) immediately after publishing.

---

## Step 8 — Shorts

1. `shorts.md` has 10 ready-to-produce Shorts per package, each with its own hook, script, and CTA.
2. Produce Shorts using the same HeyGen Avatar V clips where possible (re-cut from the long-form
   footage) or generate short-specific avatar takes for hooks that don't already exist in the long-form
   cut.
3. Apply the same sourcing discipline to Shorts as the long-form video — a Short is not exempt from the
   `[VERIFY]` flags, sensitivity exclusions, or attribution requirements just because it's short. Several
   packages explicitly flag which sensitive material (e.g. fraud-allegation specifics, sentencing
   details) must **never** be compressed into a Short without its full attribution intact — when in
   doubt, a Short should skip a sensitive detail entirely rather than compress it unsafely.
4. Publish Shorts on a staggered schedule around the long-form video's release (same day or the days
   immediately following) to drive traffic back to the full video via the CTA.

---

## Step 9 — Cross-Promotion

Same day as publish, or immediately after:

1. **Community posts:** schedule the 10 posts from `community-posts.md` over the following 1–2 weeks
   (polls, teasers, discussion prompts, behind-the-scenes notes) rather than posting them all at once.
2. **Social posts:** publish the platform-specific copy from `social-posts.md` to each channel (X,
   Threads, LinkedIn, Facebook, Instagram, TikTok, Bluesky) — adapt formatting per-platform as needed
   (e.g. thread structure on X) but the core copy is ready to use.
3. **Email:** send the "Launch Email" from `email-campaign.md` on publish day; the "Reminder Email" a
   few days later to non-openers/non-clickers; the "Final Chance Email" toward the end of the video's
   promotional push window.
4. **Blog:** publish the full article + FAQ from `blog.md` to the channel's blog/site (or Medium, or
   wherever long-form written content lives) — this is a complete, standalone SEO asset, not just a
   script transcript.
5. Fill in every `[link]`/`[Subscribe link]`/`[video link]` placeholder across all these files with the
   real, live URLs once the video is published.

---

## Step 10 — Monetization (Ongoing, Not Per-Video)

This channel's affiliate niches (per `Best affiliate products.txt`) are: cloud hosting/dev-tool
referrals (AWS/DigitalOcean partner tiers), incorporation services (Stripe Atlas–style), accounting/
runway tools, no-code platforms, fundraising/cap-table software, and startup banking referrals — B2B
SaaS affiliates commonly paying $50–$500 per conversion, the richest affiliate economics available to
this niche. Where a video's subject matter naturally overlaps one of these categories (e.g. a package
about cap-table mechanics, runway/burn-rate, or incorporation/banking decisions), place a relevant
affiliate link in the description's "Resources" section — never force an unrelated affiliate link into
a description where it doesn't fit the video's actual content.

---

## Step 11 (Optional / Phase 2) — Localization

The channel's original plan calls for expanding every English master package into 6 localized YouTube
channels: 🇺🇸 English, 🇩🇪 German, 🇫🇷 French, 🇳🇱 Dutch, 🇳🇴 Norwegian, 🇸🇪 Swedish. **This is a live,
intended initiative that has only been partially started** — only packages 004 and 009 have any
language-folder work done, and it isn't finished for either.

When resuming this work:

1. **Do not translate literally.** Translate the idea, then localize the content, then optimize for
   the target audience — the localized version should read as if a native creator wrote it, not as a
   translated English script.
2. **Preserve exactly:** meaning, facts, numbers, claims, story logic, narrative structure, emotional
   progression. Every `[VERIFY]` flag and sensitivity requirement from the English `sources-log.txt`
   carries over unchanged — localization never loosens the sourcing discipline.
3. **Adapt freely:** idioms, humor, examples, cultural references, search terminology, thumbnail
   wording, hook wording, CTA wording.
4. Each language gets its own `titles.md`-equivalent (10 localized viral + 10 curiosity + 10 SEO + 10
   high-CTR titles, ranked, with a recommended pick) — the localized title does not need to be a literal
   translation of the English one.
5. Thumbnail *concepts* stay shared across all six channels; only thumbnail *text* gets localized (e.g.
   "$150B COMPANY" → "150 Mrd. $" in German).
6. Reuse B-roll, stock footage, AI-generated images, charts, and the master editing timeline across all
   six languages wherever possible — don't regenerate identical visual assets six times unless
   localization specifically requires it.
7. Folder structure for a localized package: `0NN-Slug-Name/MASTER/` (shared research, script, sources,
   visual plan, editing timeline, thumbnail concept, assets) plus `EN/`, `DE/`, `FR/`, `NL/`, `NO/`,
   `SV/` subfolders, each containing that language's `script.md`, `title.md`, `description.md`,
   `seo.md`, `tags.md`, `subtitles.md`, `thumbnail.md`, `shorts.md`, and `social.md`.
8. Run a localization QA pass before publishing any non-English version: grammar, native fluency,
   numbers, currency, dates, names, statistics, facts, pronunciation, SEO, title length, thumbnail
   text, and cultural references. Flag anything uncertain rather than guessing.

---

## Quality Gates — Do Not Skip These

Pulled from this channel's accumulated, hard-won practice. These apply at every stage, not just
research:

- **Never state an unverified claim as fact.** If it can't be sourced, it gets a `[VERIFY]` flag or
  gets cut — never quietly upgraded to "confirmed" because it would make the story cleaner.
- **Never conflate two similarly-named or related real entities** (e.g. a parent company and a product
  it acquired, two companies with similar names, a founder and a later executive at the same company).
  Where this risk exists, every file gets an explicit standing distinction/tag.
- **Sensitive claims about real, living, non-convicted people get handled like an investigative piece,**
  not like flavor text — attributed precisely, never stated as settled fact, and cut entirely if
  they're not load-bearing to the actual story.
- **Political/legal events get strict who/what/when neutrality**, everywhere they appear, with zero
  motive speculation and zero political framing — including in Shorts and social copy, where the
  temptation to add a punchy editorial line is highest.
- **One dominant idea per thumbnail.** Never try to cram multiple beats of the story into one image.
- **No AI-generated photorealistic likenesses of real named people, and no AI-generated real company
  logos/wordmarks** — ever. Add real, rights-cleared media only in the editor.
- **When a title's premise doesn't survive the sourcing pass, say so and correct it** — in the README,
  the sources-log, and everywhere the incorrect framing would otherwise repeat. This channel corrects
  its own batch-doc titles regularly; that's expected, not a failure state.
- **Update `project_factcheck_status.md` and `project_channel_overview.md` (memory) after every
  package** — built or deliberately skipped — so future research doesn't re-litigate settled
  ground or waste time re-attempting a title that already failed a sourcing check.

---

## Quick Reference — File-to-Stage Map

```
Step 0  Pick a topic ................... (batch doc / flagged candidate / cold research)
Step 1  Research + build ............... README.md, sources-log.txt, titles.md, thumbnails.md,
                                          ai-image-prompts.md, script.md, heygen-production.md,
                                          editing-notes.md, seo.md, description.md, tags.md,
                                          hashtags.md, publishing-plan.md, shorts.md,
                                          community-posts.md, social-posts.md, email-campaign.md,
                                          blog.md  (all 18 files, in one pass)
Step 2  Pre-production review .......... README.md + sources-log.txt (read in full)
Step 3  Thumbnail (ChatGPT) ............ thumbnails.md + ai-image-prompts.md
Step 4  Video (HeyGen Avatar V) ........ script.md + heygen-production.md
Step 5  Editing ......................... editing-notes.md + script.md (chapters)
Step 6  Metadata & SEO .................. seo.md, description.md, tags.md, hashtags.md
Step 7  Publishing ...................... publishing-plan.md, community-posts.md (pinned comment)
Step 8  Shorts ........................... shorts.md
Step 9  Cross-promotion ................. community-posts.md, social-posts.md, email-campaign.md,
                                          blog.md
Step 10 Monetization ..................... Best affiliate products.txt (ongoing, not per-video)
Step 11 Localization (optional) ......... 1 Master Content Asset → 6 Localized YouTube Channels.txt
```
