# Blog Article: Twitter Cut One Startup Off On Purpose. Facebook Buried Another By Accident.

*All figures sourced to public reporting — see `sources-log.txt` for the full citation map. Where a specific figure is inconsistently reported (Viddy's exact lifetime funding total), it's flagged inline rather than stated as one precise number.*

## Introduction
"Platform risk" usually gets talked about as one thing: build on top of someone else's infrastructure, and eventually that infrastructure can be taken away. But the real historical record shows at least two distinct ways it happens, and they're not the same risk. Meerkat, a live-streaming startup that raised $14 million, had its access to Twitter's social graph deliberately cut off on the exact same day Twitter announced buying its direct rival. Viddy, a video-sharing startup that hit a $370 million valuation, watched its daily users collapse 80% in a month after Facebook changed a News Feed rule that was never aimed at Viddy specifically. One platform made a targeted decision. One platform didn't even know it was doing it. Both startups are gone. This article walks through both cases in full, including a complication that most retellings of the Meerkat story skip entirely.

## Case One: Meerkat — On Purpose

### The Breakout
Meerkat, built by Life On Air under founder and CEO Ben Rubin, broke out at SXSW 2015 as the buzziest app at the festival. Its growth mechanism depended directly on Twitter: Meerkat used Twitter's social graph so users could instantly find their Twitter friends already on the app, turning Twitter's existing social network into Meerkat's distribution engine.

### The Cutoff
On Friday, March 13, 2015 — the same day SXSW began — Twitter cut off Meerkat's access to that social graph, breaking the exact feature responsible for Meerkat's viral growth. The same day, Twitter announced it was acquiring Periscope, a live-streaming app built in-house that did almost exactly what Meerkat did. The timing wasn't a coincidence tech press missed: VentureBeat, TechCrunch, BuzzFeed News, and Engadget all covered the cutoff and the acquisition as a single, connected story in real time.

### The Raise That Happened Anyway
Two weeks after the cutoff, Meerkat closed a $14 million round led by Greylock Partners, with Josh Elman joining the board, alongside Aleph, Broadway Video Ventures, CAA Ventures, Comcast Ventures, Entree Capital, Raine Ventures, Sherpa, Slow Ventures, Sound Ventures, Universal Music Group, UTA, Vayner/RSE, and WME. That sequencing matters: investors funded Meerkat with full knowledge of what Twitter had just done, not before it happened.

### What Meerkat's Founder Actually Says
Meerkat continued operating for another 18 months before the app was officially killed in October 2016, with the team and company pivoting to a new product, Houseparty. Here's the complication most retellings skip: Ben Rubin later told TechCrunch that the decision to pivot away from Meerkat came roughly six months after launch, and that the real reason was that live broadcasting itself never became "a daily habit" for users — not primarily Twitter's API cutoff.

**Important distinction:** this is Rubin's own account, given after the fact, and it isn't independently corroborated by a second source. A founder explaining a shutdown years later has an obvious incentive to downplay how much a competitor's decision mattered. This article presents both the documented timeline (the cutoff landing the same day as the Periscope deal) and Rubin's competing explanation — without resolving the contradiction, because the public record doesn't actually resolve it either.

## Case Two: Viddy — By Accident

### The Rocket Ship
Viddy grew by riding Facebook's frictionless-sharing feature: every video posted to Viddy could automatically post to a user's Facebook Timeline, turning Facebook's News Feed into Viddy's growth engine, much like Meerkat had used Twitter's graph. Viddy reached more than 27 million registered members this way. In May 2012, Viddy closed a $30 million Series B — investors NEA, Goldman Sachs, Khosla Ventures, and Battery Ventures — at a $370 million valuation, following an earlier $2.8 million seed and $6 million Series A. (Viddy's total lifetime funding is reported inconsistently across sources, somewhere between roughly $36 million and $39.3 million — treat it as "more than $36 million" rather than one precise figure.)

### The Rule Nobody Aimed At Viddy
On May 31, 2012, Facebook rolled out what tech press called a "10-second rule" — a broad crackdown on auto-sharing spam that reduced the News Feed visibility of automatically-posted content across many apps, Viddy included. This is the detail that separates Viddy's story from Meerkat's: Facebook didn't revoke Viddy's API access or make a decision specifically about Viddy. It changed a general policy for the whole ecosystem, and Viddy simply couldn't survive being less visible in the feed that had been driving nearly all of its growth.

### The Collapse
The numbers moved fast. Viddy's daily active users fell from roughly 5 million in late April 2012 to roughly 1 million by the end of May 2012 — a drop of more than 80% in about a month. In February 2013, following a CEO departure, Viddy cut 12 staff, more than a third of its headcount.

### The Fire Sale
In January 2014, rebranded as "Supernova," Viddy was acquired by Fullscreen for $20 million — a steep comedown from the $370 million valuation it had carried just 20 months earlier. The app fully shut down in December 2014 under Fullscreen's ownership.

## The Actual Lesson: Two Failure Modes, Not One
Meerkat and Viddy are both real, well-documented casualties of platform dependency — but they illustrate two structurally different mechanisms, and conflating them misses the point of studying either case:

- **Deliberate cutoffs** happen when a platform makes a specific decision aimed at a specific company or category, usually because that company has become a competitive threat to something the platform itself wants to own. Twitter cutting off Meerkat the same day it acquired Periscope is about as clean an example of this as exists in the public record.
- **Incidental collateral damage** happens when a platform changes a broad policy for reasons that have nothing to do with any one company, and a company that happened to be heavily dependent on the old rules gets crushed as a side effect. Facebook's frictionless-sharing crackdown wasn't a decision about Viddy — it was a decision about spam, and Viddy simply couldn't survive the side effect.

The practical distinction matters for anyone building on top of a platform today: a deliberate cutoff is at least somewhat legible in advance — you can watch for competitive dynamics, acquisition rumors, or a platform building its own version of what you do. Incidental collateral damage is much harder to see coming, because by definition it isn't a decision about you at all. The only real defense against the second kind is structural: don't let any single platform's specific rules become so load-bearing to your growth that an unrelated policy change elsewhere can end your company.

## What Founders Should Take From This
- **Map your platform dependencies honestly** — which specific features, APIs, or algorithmic behaviors is your growth actually built on, not just which platforms you're "on"
- **Watch for competitive signals**, not just policy announcements — Twitter's acquisition of Periscope was the real tell for Meerkat, available before the cutoff happened
- **Assume some risk is simply unwatchable** — Viddy did nothing wrong that a policy scan would have caught; the only defense was not being so dependent on one feed algorithm in the first place
- **Distinguish the two risk types in your own planning** — a mitigation strategy built for deliberate cutoffs (diversify away from direct competitors of your platform) won't protect you from incidental collateral damage, and vice versa

## The Lesson
Building on top of a platform you don't control means accepting that the platform can end your company two different ways: on purpose, when you become a threat to something it wants to own, or by accident, when it changes a rule for reasons that were never about you. Meerkat and Viddy are real, fully-documented proof that either one is enough on its own — and neither one required the company to have done anything wrong.

## Further Reading / Sources
See `sources-log.txt` for the full citation map, including links to TechCrunch, VentureBeat, BuzzFeed News, Engadget, CNN Money, Los Angeles Business Journal, Recode, and Variety coverage of both cases.

---

# FAQ (30 Questions)

**1. What happened to Meerkat?**
Meerkat, a live-streaming app, broke out at SXSW 2015. On March 13, 2015, Twitter cut off its access to Twitter's social graph — the same day Twitter announced acquiring Meerkat's rival, Periscope. Meerkat raised $14M two weeks later, operated another 18 months, and shut down in October 2016, pivoting its team to a new product, Houseparty.

**2. Did Twitter kill Meerkat?**
Twitter's cutoff clearly damaged Meerkat's core growth mechanism and happened the same day as a directly competing acquisition — that timing is well documented. But Meerkat's own founder, Ben Rubin, later said the real reason for the pivot was that live broadcasting never became a daily habit for users, not primarily the API cutoff. Both are part of the real record; neither fully resolves the other.

**3. What happened to Viddy?**
Viddy, a video-sharing app, hit a $370 million valuation on a $30M Series B in May 2012. A Facebook anti-spam algorithm change in May 2012 — not aimed at Viddy specifically — cut its News Feed visibility. Its daily active users fell from about 5 million to about 1 million in roughly a month. It fire-sold for $20 million in January 2014 and fully shut down in December 2014.

**4. Did Facebook target Viddy specifically?**
No. Facebook's May 2012 "10-second rule" was a broad policy change aimed at auto-sharing spam across many apps, not a decision about Viddy. Viddy was affected as a side effect of a general rule change.

**5. How much did Meerkat raise?**
$14 million, announced March 26, 2015, led by Greylock Partners.

**6. How much did Viddy raise?**
A $2.8M seed, a $6M Series A (Feb 2012), and a $30M Series B (May 2012) that valued it at $370M. Total lifetime funding is reported inconsistently across sources, roughly $36M–$39.3M.

**7. What is a social graph API?**
A feature that lets an app access a platform's existing network of user connections — in Meerkat's case, Twitter's follower/following relationships — so new users can instantly find people they already know on the new app.

**8. What is frictionless sharing?**
A Facebook feature (part of Open Graph) that let apps automatically post a user's activity — like a video watched or shared — to their Facebook Timeline without a manual share action each time.

**9. What was Facebook's "10-second rule"?**
A May 2012 Facebook policy change cracking down on auto-sharing spam, which reduced the News Feed visibility of automated posts from apps like Viddy that relied heavily on frictionless sharing for distribution.

**10. What happened to Meerkat's team after the shutdown?**
They pivoted the company, Life On Air, to a new product called Houseparty.

**11. Who bought Viddy?**
Fullscreen acquired Viddy (rebranded as "Supernova") for $20 million, announced January 2014.

**12. Is the "40 startups" figure from the original version of this video's title real?**
No — no sourced count of "40 startups" killed by any single API/platform event was found in research for this video, and that framing has been dropped entirely in favor of two fully-verified, named cases.

**13. What's the difference between Meerkat's and Viddy's situations?**
Meerkat's was a deliberate, targeted access cutoff tied to a competing acquisition. Viddy's was a broad policy/algorithm change that hit Viddy as a side effect, not a decision aimed at Viddy.

**14. Is it accurate to call what happened to Viddy an "API shutdown"?**
Not literally — Facebook didn't revoke Viddy's API access the way Twitter revoked Meerkat's. It changed a News Feed visibility/ranking rule broadly. This video is explicit about that distinction rather than flattening both stories into "an API shutdown."

**15. Who invested in Meerkat besides Greylock?**
Aleph, Broadway Video Ventures, CAA Ventures, Comcast Ventures, Entree Capital, Raine Ventures, Sherpa, Slow Ventures, Sound Ventures, Universal Music Group, UTA, Vayner/RSE, and WME.

**16. Who invested in Viddy's Series B?**
NEA, Goldman Sachs, Khosla Ventures, and Battery Ventures.

**17. When exactly did Twitter cut off Meerkat?**
Friday, March 13, 2015 — the same day Twitter announced acquiring Periscope, and the same day SXSW 2015 began.

**18. When exactly did Viddy's daily users collapse?**
From roughly 5 million (late April 2012) to roughly 1 million (end of May 2012) — about a month.

**19. Was Meerkat's $14M raise before or after the Twitter cutoff?**
After — the round closed roughly two weeks after Twitter had already cut off Meerkat's social graph access.

**20. What happened to Socialcam — wasn't it in the same situation as Viddy?**
No — Socialcam sold to Autodesk for $60 million in August 2012 while it was still the #1 Facebook app, and ran three more years before shutting down in 2015 for unrelated reasons. It's not presented as a casualty of the same mechanism that hit Viddy.

**21. Did the 2018 Google Maps pricing change or the 2023 Twitter API paywall kill any funded startups?**
Research for this video found no specific, named, VC-funded startup whose death is reliably and directly attributed to either event in the public record — both are real events, but neither had a clear funded-company casualty to anchor a segment on.

**22. What is venture platform dependency risk?**
The risk that a company's core growth or product functionality depends on continued access to a third-party platform's API, data, or distribution mechanism — access the platform can change or revoke for its own reasons.

**23. Can you protect against a deliberate platform cutoff?**
Partially — watching for competitive signals (a platform building or acquiring something similar to what you do) can give some warning, though it doesn't guarantee protection.

**24. Can you protect against incidental algorithm-driven collateral damage?**
Only structurally — by not making any single platform's specific rules so load-bearing to your growth that an unrelated policy change elsewhere can end your company.

**25. What happened to Ben Rubin after Meerkat?**
He continued leading Life On Air through its pivot to Houseparty.

**26. Where do you get the information for these videos?**
Public press coverage (TechCrunch, VentureBeat, BuzzFeed News, Engadget, CNN Money, Los Angeles Business Journal, Recode, Variety), founders' own later statements, cited on screen and linked in the description and sources log.

**27. What other startups have you covered?**
See the channel's "Startup Autopsies" playlist.

**28. Can I suggest a similar platform-risk case for a future video?**
Yes — leave your suggestion in the comments.

**29. What's the single biggest lesson from this video for founders?**
Map exactly which platform features your growth depends on, and understand that "platform risk" is at least two different risks — one you can sometimes see coming, and one you usually can't.

**30. What's the main takeaway from this video?**
A platform doesn't have to be trying to kill your company to kill it — deliberate targeting and incidental policy collateral damage are both fatal, and they require different defenses.
