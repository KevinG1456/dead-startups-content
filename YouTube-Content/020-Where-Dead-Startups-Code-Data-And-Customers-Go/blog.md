# Blog Article: Where Dead Startups' Code, Data, and Customers Actually Go (The Liquidation Supply Chain)

*The Sidecar/GM, RadioShack, and Cambridge Analytica cases below are real, reported examples — confirm current figures and legal details against primary sources (court filings, press coverage) before publishing. The "abrupt SaaS shutdown" pattern is an illustrative composite, not a single named company, and is labeled as such.*

## Introduction
When a startup "shuts down," the announcement typically treats it as a single event — one company, one ending. In reality, a dead startup splits into three separate supply chains: its code and intellectual property, its customer data, and its customer relationships. Each follows its own legal and commercial pathway to a new destination, and almost none of it is explained to the people who built, worked at, or used the product. This article maps all three tracks, grounded in real, documented cases.

## Track 1: Where the Code Goes
When a startup fails, its codebase and intellectual property don't necessarily die with it. Two common outcomes dominate: an **acqui-hire**, where an acquiring company primarily wants the founding/engineering team, typically discontinuing the original product shortly after; and an **asset sale**, where specific assets — including patents — are sold off separately, sometimes to a buyer with no connection to the original product at all.

Ride-share startup **Sidecar** shut down at the end of 2015. **General Motors** acquired its technology and assets and hired roughly 20 of its employees — an acqui-hire and asset purchase, not a pure IP sale — with a *license* to Sidecar's patents (Sidecar retained ownership) as a key component of the deal `[VERIFY exact deal terms/value]`. The more interesting detail: GM wasn't an unrelated buyer picking up orphaned IP. The deal closed just two weeks after GM's $500 million investment in Lyft, as part of the same strategic push against Uber — GM described the two deals as officially unconnected, but the timing tells its own story. It's a useful reminder that even a transaction that reads as a clean, arm's-length asset sale often has a strategically motivated buyer behind it. More broadly (and separately from the Sidecar case), patent-assertion entities ("patent trolls") are known to acquire failed startups' patent portfolios cheaply during liquidation, sometimes later asserting them offensively against unrelated companies — a well-documented industry pattern.

## Track 2: Where the Data Goes
Customer and user data is legally treated as a company asset — one that can be sold in a bankruptcy proceeding, even when a privacy policy promised it never would be.

The clearest illustration is **RadioShack's 2015 bankruptcy**. RadioShack attempted to sell its customer database — reportedly containing tens of millions of customer records — as part of its bankruptcy asset sale `[VERIFY exact record count]`. Multiple state attorneys general objected, pointing directly to RadioShack's own privacy policy, which had promised customer data would never be sold. A court-approved settlement significantly restricted the sale `[VERIFY exact settlement terms]`. This case remains the most-cited precedent for how bankruptcy courts and regulators now treat customer data as a liquidation asset — and it's part of why some bankruptcy courts require the appointment of a **consumer privacy ombudsman** (the role itself created by 11 U.S.C. §332, triggered when §363(b)(1) requires a hearing) when a proposed data sale conflicts with a company's existing privacy policy.

A second case shows a different kind of regulatory intervention — one worth distinguishing from RadioShack's. After **Cambridge Analytica** collapsed amid the Facebook data scandal and filed for bankruptcy in May 2018, the **FTC** pursued a separate Section 5 enforcement action for deceptive data-collection practices, culminating in a December 2019 final order requiring the company to delete the improperly obtained Facebook data and associated work product `[VERIFY exact FTC action and timeline]`. Unlike RadioShack, this wasn't a bankruptcy-court data-sale under review — it was independent regulatory enforcement running alongside the bankruptcy, not a §363 asset-sale process.

## Track 3: Where the Customers Go
The people who actually used the product face a spectrum of outcomes, from graceful to abrupt.

At the graceful end: **Parse**, Facebook's mobile backend-as-a-service, shut down in 2017 with roughly a year's notice, open-sourced its server software (Parse Server), and gave customers a structured path to self-host and migrate their apps `[VERIFY exact shutdown timeline]`. At the more common, illustrative end of the spectrum: many B2B SaaS shutdowns give customers only a short window — commonly reported as around 30 days — to export their data before access is cut off entirely, sometimes leaving business customers scrambling.

## What to Check Before You Trust a Startup With Your Data
For users and B2B buyers: check whether a company's privacy policy addresses what happens to data in the event of a shutdown, acquisition, or bankruptcy — not just day-to-day data handling. For founders navigating a wind-down: understand that a privacy policy promising never to sell data can still be legally tested in a bankruptcy sale, and that proactively offering a real data-export or migration path (as Parse did) is both an ethical and reputational choice, not a legal requirement in most cases.

## The Lesson
A startup's death isn't a single ending — it's a fork into three separate supply chains, each with its own legal mechanics and its own destination. Understanding where the code, the data, and the customers actually go matters for founders planning a wind-down, for employees and investors evaluating what "acquired" or "shut down" really means, and for every user who has ever trusted a startup with their data.

## Further Reading / Sources
- `[Sidecar/General Motors deal reporting — link]`
- `[RadioShack bankruptcy data-sale settlement reporting — link]`
- `[Cambridge Analytica FTC bankruptcy action — link]`
- `[Parse shutdown/migration announcement — link]`

---

# FAQ (30 Questions)

**1. What happens to a startup's code when it shuts down?**
It typically goes one of two ways: an acqui-hire (the team, and sometimes the codebase, join an acquirer, with the original product usually discontinued) or an asset sale (specific assets, including patents, sold off separately).

**2. What happens to a startup's customer data when it shuts down?**
It's legally treated as a company asset that can potentially be sold, transferred to an acquirer, or deleted — the outcome depends on bankruptcy proceedings, the company's privacy policy, and sometimes regulatory intervention.

**3. Is a company allowed to sell customer data even if its privacy policy says it won't?**
It's legally contested territory — the RadioShack case is the landmark example of this exact conflict, and some bankruptcy courts now require a consumer privacy ombudsman review in these situations.

**4. What is a consumer privacy ombudsman?**
A court-appointed role in certain bankruptcy proceedings, created under 11 U.S.C. §332 and triggered when §363(b)(1) requires a hearing because a proposed data sale conflicts with a company's existing privacy policy, tasked with evaluating the privacy implications of the sale.

**5. What happened with RadioShack's data sale?**
RadioShack attempted to sell its customer database in its 2015 bankruptcy; multiple state attorneys general objected citing the company's own privacy policy, and a settlement significantly restricted the sale.

**6. What happened with Sidecar's patents?**
The ride-share startup shut down in 2015; General Motors acquired its technology and assets and hired about 20 employees, with a license to Sidecar's patents (Sidecar kept ownership) as part of the deal — closing two weeks after GM's $500M investment in Lyft.

**7. What is an acqui-hire?**
An acquisition primarily aimed at bringing an acquired company's team onto the acquirer's payroll, with the original product usually discontinued shortly after.

**8. What is an asset sale?**
A liquidation process where a company's specific assets (code, patents, customer lists, equipment) are sold off individually, rather than the company being acquired as a going concern.

**9. What happened with Cambridge Analytica's bankruptcy?**
Separately from the May 2018 bankruptcy filing, the FTC pursued its own Section 5 enforcement action for deceptive data practices, resulting in a December 2019 order requiring deletion of the improperly obtained Facebook data — a distinct process from a bankruptcy-court-supervised asset sale like RadioShack's.

**10. What happened when Parse shut down?**
Facebook gave Parse customers roughly a year's notice, open-sourced the Parse Server software, and provided a structured path for customers to self-host and migrate their apps.

**11. Is my data automatically deleted when a startup shuts down?**
Not necessarily — deletion is one possible outcome among several, alongside transfer to an acquirer, sale as a bankruptcy asset, or in some cases, simple neglect.

**12. What is a patent-assertion entity?**
Often called a "patent troll," a company that acquires patents (sometimes cheaply from failed startups) primarily to assert them against other companies rather than to build products.

**13. How much notice do SaaS companies typically give before shutting down?**
It varies significantly — some, like Parse, give roughly a year; many others give considerably less, commonly reported around 30 days for data export.

**14. What should I check in a privacy policy about shutdown scenarios?**
Whether it addresses what happens to your data specifically in the event of a shutdown, acquisition, or bankruptcy — not just routine data handling.

**15. What should B2B buyers ask startup vendors about shutdown risk?**
Whether there's a documented data-export or migration plan, and what happens to their data and integrations if the vendor is acquired or shuts down.

**16. Does bankruptcy law treat customer data the same as other company assets?**
Largely yes, though special protections (like the consumer privacy ombudsman requirement) can apply when a privacy policy conflicts with a proposed sale.

**17. Can a dead startup's patents be used against unrelated companies later?**
Yes — this is the general pattern with patent-assertion entities acquiring dead startups' patent portfolios and later asserting them offensively.

**18. Is this video sponsored by or affiliated with RadioShack, GM, or any company mentioned?**
No — this is an independent educational explainer referencing public, reported information for context.

**19. Where do you get the information for these videos?**
Public court filings, press coverage, and regulatory actions, cited and linked in the description.

**20. What other startups have you covered?**
See the channel's "Startup Autopsies" playlist.

**21. Can I suggest a real shutdown/liquidation example for a future video?**
Yes — leave your suggestion in the comments.

**22. What's the single biggest lesson from this video for users?**
Check what a company's privacy policy actually says about shutdown, acquisition, and bankruptcy scenarios — not just routine data use.

**23. What's the single biggest lesson from this video for founders?**
A privacy policy promising never to sell data can still be tested in a bankruptcy sale — plan your wind-down and communicate with customers proactively, the way Parse did.

**24. Does a company need my consent to transfer my data to an acquirer?**
It depends on jurisdiction and the specific privacy policy/regulatory framework (e.g., GDPR and CCPA impose additional requirements) — this varies and isn't guaranteed either way.

**25. What is contract assignment in the context of a startup shutdown?**
The transfer of a company's existing customer contracts to an acquiring company, allowing the acquirer to take over those customer relationships — subject to the contract's own assignment terms.

**26. Are all startup shutdowns handled this poorly?**
No — Parse is a clear counterexample of a well-handled, well-communicated shutdown with a real migration path.

**27. Does this topic relate to the "Acquired for $1" video?**
Yes — both explore what "acquired" or "shut down" actually means mechanically, beyond the headline; they pair well as a "startup legal mechanics" mini-series.

**28. What is GDPR/CCPA's relevance to startup data liquidation?**
Both frameworks impose additional obligations (such as deletion rights and restrictions on data transfer) that can complicate or restrict a straightforward data sale during a shutdown, particularly for companies with EU or California users.

**29. How can founders handle a shutdown responsibly?**
Give customers as much advance notice as possible, provide a real data-export or migration path, and be transparent about what will happen to customer data specifically.

**30. What's the main takeaway from this video?**
A startup's death isn't one event — it's a fork into three separate supply chains for its code, its data, and its customers, each with its own legal mechanics and destination.
