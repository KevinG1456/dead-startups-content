# Script Package

Cyanogen and Docker figures must be confirmed against primary sources before recording. The "open-core risk spectrum" (Died / Distressed Sale / Survived) is this video's core organizing visual — keep it on screen or referenced throughout.

---

## 20 Hooks

1. **(Curiosity)** "This company raised over $100 million. Then its own free software killed it."
2. **(Curiosity)** "The free version of their product didn't just compete with them. It won."
3. **(Fear)** "If you're building an open-source company, this is the failure mode nobody warns you about."
4. **(Fear)** "This is what happens when your own community stops needing you."
5. **(Story)** "In 2013, a startup set out to build a rival to Google's Android. By 2017, it barely existed."
6. **(Story)** "Docker's technology is on almost every server on Earth. Docker the company nearly didn't survive that."
7. **(Statistics)** "One of these companies raised over $100 million. The free thing it gave away outlived it."
8. **(Statistics)** "Docker Inc. was once valued at over a billion dollars. It sold its core business for undisclosed terms — widely seen as a fraction of that."
9. **(Mystery)** "There's a version of failure where the product succeeds completely and the company still dies."
10. **(Mystery)** "The software this company built is still running today. The company itself isn't."
11. **(Question)** "What happens when the free version of your product is just as good as the paid one?"
12. **(Question)** "Can giving your product away for free actually be what kills your company?"
13. **(Controversy)** "Open source didn't save these companies. In one case, it's the exact thing that killed one."
14. **(Controversy)** "Everyone treats open source as pure goodwill. For at least one company, it was a business model mistake."
15. **(Emotional)** "They built something people genuinely loved. It still wasn't enough to save the company."
16. **(Emotional)** "This is what it's like to lose a company to the exact thing you built it around."
17. **(Authority)** "I reconstructed what actually happened to 2 companies that lost to their own open-source projects."
18. **(Authority)** "Here's the exact mechanism that let a free fork outlive a $100M+ company."
19. **(Challenge)** "Guess which of these well-known technologies is still free and everywhere today — while the company behind it nearly disappeared."
20. **(Curiosity)** "The open-source project that killed its own company. Here's exactly how it happened."

**Recommended hook for main cut:** #1 combined with #20.

---

## Complete Viral Script (Main Cut)

**Target length:** 11–14 minutes

### Cold Open (0:00–0:20)
- VO: "This company raised over $100 million. Then its own free software killed it."
- Visual: the two-box free-vs-company graphic animates in, the "company" box cracking and dimming, heavy SFX hit
- Pattern Interrupt: hard cut to silence, white text on black: "This isn't a story about a bad idea. It's a story about a business model trap."

### The Setup: What Is the Open-Core Dilemma (0:20–1:40)
- Plain-language definition: when a company builds its business on top of a free, open-source project, and the free version ends up doing everything most users actually need
- Preview: this video walks through two real companies on opposite ends of that risk — one that died from it, one that nearly did — and one pair of companies that saw it coming and fought back

### Case 1: Cyanogen Inc. (1:40–5:00)
- The pitch: in 2013, Cyanogen Inc. set out to commercialize Cyanogen OS, built on top of the already-popular free, open-source CyanogenMod project — by January 2015, CEO Kirt McMaster was publicly talking about wanting to "take Android away from Google"
- The raise: `[VERIFY exact figures]` reportedly over $100M across multiple rounds from investors including Andreessen Horowitz, Twitter co-founders, Qualcomm, Telefónica, and Rupert Murdoch
- The problem: CyanogenMod — the free, community-maintained version — kept existing, kept improving, and did nearly everything Cyanogen OS did, for free, with no commercial strings attached
- The collapse: large layoffs through 2016, Cyanogen OS and nightly build support discontinued by the end of 2016
- The twist (visual centerpiece of this segment): the volunteer community immediately forked CyanogenMod into LineageOS — which is still actively maintained today. The free project outlived the $100M+ company that tried to commercialize it.
- Visual: timeline graphic building year by year, ending on the LineageOS fork moment with a "STILL ACTIVE TODAY" label

### Case 2: Docker Inc. (5:00–8:30)
- The setup: Docker's open-source container engine became the industry-standard way to package and ship software — adopted for free almost everywhere in the industry
- The problem: the free engine did what most developers actually needed, and the layer where real enterprise revenue lived — orchestration — was won by other free, open-source tools (chiefly Kubernetes) rather than Docker's own paid Swarm/Enterprise products
- The numbers: Docker Inc. reportedly reached a valuation of roughly `[VERIFY: ~$1.3B, 2016–2018 rounds]`, then sold its entire enterprise business to Mirantis in November 2019; the deal terms were never disclosed `[VERIFY: confirm no terms were ever made public]`
- The distinction from Case 1: Docker Inc. didn't die — it survived by shrinking down to a smaller, developer-subscription-focused company (Docker Desktop, Docker Hub), helped by a simultaneous $35M raise from returning backers Benchmark and Insight Partners — this is a "distressed sale, not a shutdown," and it eventually found sustainable revenue
- Visual: valuation-vs-time line graph that drops sharply at the Mirantis sale point, then a smaller stable line continuing afterward

### Mid-video CTA (8:30)
- "If you're building — or investing in — anything with an open-source or open-core business model, the next part is the part that actually matters for you. Subscribe for a new autopsy every week."

### Case 3: MongoDB and Elastic vs. AWS — The Companies That Fought Back (8:30–11:00)
- The same risk from a different angle: cloud providers, mainly AWS, began offering fully hosted versions of MongoDB's and Elasticsearch's own open-source databases — with AWS capturing the hosting revenue instead of the companies that built and maintained the projects
- The response: MongoDB moved to the Server Side Public License (SSPL) in 2018; Elastic followed in 2021, explicitly citing the same competitive pressure
- The consequence: AWS forked Elasticsearch into OpenSearch in 2021 rather than comply with the new license
- The outcome: both companies are public (Nasdaq: MDB, NYSE: ESTC) and survived — included here specifically to show the same underlying mechanism from Cases 1 and 2, but caught and fought before it became fatal
- Visual: the open-core risk spectrum graphic completes here — "Died" (Cyanogen) / "Distressed Sale" (Docker) / "Survived by Fighting" (MongoDB/Elastic)

### Why This Happens — The Mechanism, Named (11:00–12:15)
- Plain-language synthesis: the risk isn't "open source" itself — Red Hat has run a profitable open-source business for decades by selling support and a stable enterprise distribution on top of free code, not a feature-identical free substitute
- The actual risk is specific: when the free version is not meaningfully different from what most paying customers would need, the free version doesn't support the company — it replaces the reason to pay it

### Final CTA + Outro (12:15–13:15)
- VO: recap the one-sentence lesson — giving away your product for free isn't inherently risky, but giving away a product that fully substitutes for what you're trying to sell can be an existential decision most founders don't recognize as one until it's too late
- "Subscribe — I'm building a full library of these"
- Engagement prompt: "If you've ever chosen the free, open-source version of a paid product instead of paying for it — which one, and why? Comment below."
- End screen: two related autopsies + subscribe

---

## Alternative Scripts

### Script Version A — Data-First / Analyst Style
Opens directly on the completed open-core risk spectrum graphic (Died / Distressed Sale / Survived), then works backward chronologically through each case in detail. Measured, graphics-forward, treats the video as a genuine business-strategy resource for founders and investors.

### Script Version B — Narrative / Documentary Style
Opens on the human moment — Kirt McMaster's 2015 "take Android away from Google" quote, played for irony against what actually happened — before any numbers appear. Slower pacing, more narrative-driven, ends on the LineageOS-still-exists twist as the emotional climax rather than a mid-video beat.

### Script Version C — Fast-Cut / Listicle Style
Structured as "3 companies, 3 outcomes, 1 mistake that connects them," each case covered in under 2 minutes with the risk spectrum graphic building incrementally after each one. Strong Shorts-extraction potential.

---

## Audience Retention Optimization
- **Drop-off risk:** the Docker segment (5:00–8:30) if it becomes too technical about orchestration/Kubernetes without staying grounded in the business/valuation story
- **Fix:** keep the technical detail minimal — one sentence on "why Kubernetes won instead of Swarm" is enough; the segment's job is the valuation-to-distressed-sale arc, not a container-orchestration explainer
- **Faster pacing opportunity:** if audience feedback suggests strong familiarity with Docker's story already, compress Case 2 and spend more time on the less-widely-known Cyanogen/LineageOS twist
- **Curiosity increase opportunity:** tease the LineageOS-still-exists fact in the cold open or title-card preview to sustain interest through the setup section
- **Recommended visual change:** keep the open-core risk spectrum graphic building incrementally and visible in a corner throughout, so viewers always know where each case sits on the spectrum

---

## Chapters / Timestamps
- 00:00 Cold Open
- 00:20 The Setup: What Is the Open-Core Dilemma
- 01:40 Case 1: Cyanogen Inc. and CyanogenMod
- 05:00 Case 2: Docker Inc.
- 08:30 Mid-Video: Why This Matters If You're Building or Investing in Open Source
- 08:35 Case 3: MongoDB and Elastic vs. AWS
- 11:00 Why This Happens — The Mechanism, Named
- 12:15 What's Next
