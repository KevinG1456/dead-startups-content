# 020 — Where Dead Startups' Code, Data, and Customers Actually Go (The Liquidation Supply Chain)

**Package status:** Structural framework ready. This is a legal/mechanism explainer video, not a single-company autopsy — its job is to demystify what actually happens to a startup's three core assets (its code/IP, its customer data, and its customer relationships/contracts) once the company shuts down or is sold off. Anchored by real, well-documented cases; grounded in general, verifiable legal/bankruptcy mechanics rather than any single company's confidential records.

**Real anchor examples to use (verify current figures/details before recording):**
1. **Sidecar (ride-share startup)** — shut down at the end of 2015; General Motors acquired its technology and assets and hired roughly 20 of its employees, with a *license* to Sidecar's patent portfolio (Sidecar retained ownership) as a key component of the deal. GM was not an unconnected buyer picking up orphaned IP — the deal closed just two weeks after GM's $500M investment in Lyft, as part of the same ride-sharing strategy against Uber (GM described the two deals as officially unconnected, but the timing is notable). Illustrates a more nuanced version of Track 1's point: what looks like a clean IP carve-out to an outside buyer is often actually an acqui-hire plus a strategically-motivated license, not a simple sale to an unrelated party `[VERIFY exact deal terms/value]`.
2. **RadioShack's 2015 bankruptcy — the landmark data-sale precedent.** RadioShack attempted to sell its customer database (reportedly tens of millions of customer records) as a bankruptcy asset; multiple state attorneys general objected, citing RadioShack's own privacy policy promising never to sell customer data, and a court-approved settlement significantly restricted the sale. Not a funded startup, but this is the single most-cited precedent shaping how bankruptcy courts and regulators now treat customer data as a liquidation asset — directly relevant to every funded startup that shuts down holding a user database `[VERIFY exact record count and settlement terms]`.
3. **Cambridge Analytica's 2018 bankruptcy** — after the company collapsed amid the Facebook data scandal, the FTC took action during the bankruptcy process specifically to prevent the improperly-obtained user data from simply being sold off or repurposed by successor entities — a rare, well-documented case of a regulator intervening directly in the data-liquidation pipeline `[VERIFY exact FTC action and timeline]`.
4. **Parse (Facebook's mobile backend-as-a-service)** — shut down in 2017 with roughly a year's notice, open-sourced its server software (Parse Server), and gave customers a structured self-hosting migration path — the closest real example of a "graceful" liquidation, useful as the contrast case against abrupt shutdowns that strand customers with little notice `[VERIFY exact shutdown timeline]`.

**Framing requirement:** never assert confidential internal details (a specific company's actual customer count sold, actual patent sale price, etc.) unless directly sourced to a primary document (bankruptcy court filing, press release, SEC filing, confirmed news reporting) — use "reportedly," cite the source, and flag unverified figures with `[VERIFY]` rather than presenting them as confirmed fact. This is a mechanism video first, case-study video second: the legal/structural explanation (asset sales, Section 363 bankruptcy sales, data privacy ombudsman requirements, contract assignment clauses) must be accurate and general even where a specific illustrative number is approximate.

---

## 1. Title Analysis

| Dimension | Assessment |
|---|---|
| Core idea | The "liquidation supply chain" — a startup's code/IP, customer data, and customer relationships don't simply vanish when it dies; they flow through specific, largely invisible legal and commercial pathways to new owners |
| Search intent | Medium-high — "what happens to a company's data when it shuts down," "startup shutdown data privacy," and "acqui-hire vs asset sale" are active, recurring searches, especially spiking after high-profile shutdowns |
| Audience intent | Founders shutting down or considering a wind-down want to know their legal obligations; employees/customers of a dying startup want to know what happens to their data and access; B2B buyers evaluating vendor risk want to understand what happens if a vendor dies |
| Emotional triggers | Unease (your data outlives the relationship you thought you controlled), curiosity (a genuinely under-explained mechanical process), validation (confirms the vague suspicion that "my data probably didn't just disappear") |
| Curiosity level | High — most viewers have never thought concretely about where a dead startup's assets physically/legally go, and the video promises to map an invisible process |
| Competition level | Low — this specific angle (code + data + customers as three distinct liquidation tracks) is rarely covered as a unified explainer; adjacent coverage exists in privacy journalism and bankruptcy-law content, but not aimed at this audience in this format |
| Viral potential | Medium-high — strong "wait, what actually happens to MY data" hook that applies to nearly every viewer who has ever used a startup product that later shut down |
| Evergreen score | High — startup shutdowns are constant and the underlying legal mechanics (asset sales, bankruptcy data-sale rules, contract assignment) don't change often |
| Suggested improvement | Build a single reusable "liquidation supply chain" flow diagram (code → acquirer/patent buyer, data → bankruptcy sale/ombudsman review/deletion, customers → migration/stranding) as the video's signature visual — highly shareable and screenshot-worthy on its own |

**Stronger angle to consider:** Frame a meaningful chunk of the video around direct viewer self-interest — "here's how to check what actually happens to your data the next time an app you use shuts down" — turning an abstract mechanism explainer into something with immediate personal utility, which tends to outperform pure business-mechanics framing for general audience reach.

---

## 2. Viewer Psychology
- **Curiosity triggers:** the specific legal mechanics of what happens to code, data, and customers separately (most viewers assume "the company" is one indivisible thing that just disappears); what a "data privacy ombudsman" in bankruptcy actually is
- **Emotional triggers:** mild unease/betrayal (a privacy policy promising never to sell your data can still end up being tested against a bankruptcy sale), validation (confirms the intuition that dead-startup data doesn't simply vanish)
- **Viewer objections:** "isn't my data just deleted when a company shuts down?" — address directly by explaining that deletion is one possible outcome among several (asset sale, transfer to acquirer, regulator-mandated deletion, quiet neglect/security risk), not the default
- **Motivation to watch:** general self-interest (nearly everyone has used a product from a company that later died), practical value for founders navigating a wind-down and for B2B buyers assessing vendor risk
- **Expected comments:** people naming specific dead apps and asking what happened to their data, founders sharing their own wind-down experiences, requests for a "how to check" follow-up guide

## 3. Competitor Analysis
- **Similar creators:** privacy-focused journalism (Wired, The Markup) and bankruptcy-law content occasionally cover data-sale controversies case by case; almost nobody has unified code + data + customers into one structural "supply chain" framework aimed at a startup-world audience
- **Content gap:** no widely-known video explainer walks through all three liquidation tracks (IP, data, customers) as one coherent system with a reusable visual framework
- **How to outperform:** build and reuse the liquidation-supply-chain diagram as a recurring channel asset, and ground it in named, sourced real cases rather than staying abstract

## 4. Performance Prediction

| Metric | Estimate | Why |
|---|---|---|
| CTR | 6–8% | Strong "wait, where does MY data actually go" curiosity hook with broad applicability beyond the core niche |
| Retention | Strong if each of the three tracks (code/data/customers) stays visually concrete and example-driven rather than becoming a dry legal lecture |
| Engagement | Medium-high — broad relatability (everyone has used a since-shutdown product) plus strong niche relevance for founders and vendor-risk-conscious B2B buyers |
| Search Performance | Good, sustained relevance for "what happens to startup data when it shuts down" and "acqui-hire vs asset sale" search terms |

## 5. Improvement Suggestions
- Confirm the Sidecar/GM deal terms (patent license value, employee count) and the RadioShack settlement details precisely before recording — these are the load-bearing factual anchors
- Build the liquidation-supply-chain diagram as a clean, standalone, highly shareable visual asset (works well as a single image post or Short on its own)
- Include a short practical segment: "how to check what happens to your data before a startup you use shuts down" — gives the video direct viewer utility beyond the explainer content

---

## Package Contents
See `titles.md`, `thumbnails.md`, `ai-image-prompts.md`, `script.md`, `heygen-production.md`, `seo.md`, `description.md`, `tags.md`, `hashtags.md`, `shorts.md`, `community-posts.md`, `social-posts.md`, `email-campaign.md`, `blog.md`, `editing-notes.md`, `publishing-plan.md`.
