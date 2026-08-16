# Blog Article: Facebook Killed This Company in 2017. Its Code Has More Users Today Than It Ever Did.

*All figures sourced to Wikipedia, TechCrunch, VentureBeat, and the Parse Server GitHub repository
— see `sources-log.txt` for the full citation map. This article covers a genuinely different kind
of story for this series: a company that died, and an outcome that's arguably better than most of
the companies still alive.*

## Introduction
Most stories on this channel end the same way: a company runs out of runway, gets acquired and
quietly killed, or collapses under its own weight, and whatever it built disappears with it.
Parse, Inc. is the exception. The company is dead. What it built isn't — and by most measures,
it's doing better today than the company ever did.

## The Founding
Parse was founded in 2011 by Ilya Sukhar, James Yu, Tikhon Bernstam, and Kevin Lacker, part of Y
Combinator's Summer 2011 batch. It built a mobile Backend-as-a-Service platform — cloud data
storage, user authentication, push notifications, and hosted custom code — at a moment when nearly
every mobile app developer had to build that infrastructure from scratch. One of its four
co-founders, Tikhon Bernstam, had already co-founded Scribd five years earlier, in Y Combinator's
Summer 2006 batch — the sole survivor of the eleven-company batch this channel fully audited in an
earlier video.

## The Acquisition
Parse raised roughly $7-8.5 million (sources disagree slightly on the exact figure — see
`sources-log.txt`) before Facebook acquired it on April 25, 2013, for a reported ~$85 million in a
part-cash, part-stock deal. Facebook positioned it as its first-ever paid B2B product — a notable
detail, since Facebook wasn't otherwise in the business of selling developer tools for revenue at
the time. Parse operated and grew as Facebook's developer platform for roughly three years.

## The Announcement
In January 2016, Facebook announced it would sunset the hosted Parse.com service. This is where
most acquisition stories on this channel turn grim — but here, the shutdown date wasn't immediate.
Facebook set it a full year out: January 28, 2017.

## The Part That Matters
At the exact moment of the shutdown announcement, Facebook did something almost no acquirer does:
it open-sourced the entire Parse backend as "Parse Server," a Node.js project any developer could
run on their own infrastructure — AWS, Google Cloud, a personal server, anywhere. It was framed
explicitly as a migration path, not a parting gesture. The large majority of Parse's existing
customers used it to move their apps off Parse.com without having to rebuild from scratch.

## Exactly on Schedule
January 28, 2017 — Parse.com shut down exactly on the date announced a year earlier. No surprise
extension, no quiet delay, no abrupt early cutoff. It happened precisely when Facebook said it
would.

## Nine Years Later
Here's the actual point of this story. Parse Server has been continuously, independently
maintained since 2017 by a community organization — not Facebook, which has had no ongoing
involvement for almost a decade. As of this writing in 2026: Parse Server has 21,407+ GitHub
stars, active commits within the past year, and documented support for current Node.js versions
extending through 2028. Companies are still running it in production today. The company that built
it has been dead for nine years. The code is, by every available measure, more actively maintained
right now than most software from companies that are still operating.

## Died vs. Won
It's worth being precise about what actually happened here, because it's easy to blur the two
halves of this story together. The company died — completely, permanently, with no ambiguity.
Facebook shut it down, on schedule, in 2017, and has had nothing to do with it since. But the idea
Parse built — a simple, open, self-hostable mobile backend — didn't die with it. It kept growing,
under different stewardship, for reasons that have nothing to do with the original company's
survival.

## A Different Kind of Acqui-Hire
This channel has also covered Mailbox, an email app Dropbox acquired in 2013 for a reported ~$100
million, then let quietly wither with almost no updates before killing it in 2015-2016 — leaving
nothing behind for its users. Same broad shape (venture-backed startup, acquired by a much larger
company, eventually killed), completely different outcome. The difference wasn't the acquisition.
It was what the acquirer chose to do on the way out.

## The Actual Lesson
The lesson here isn't "open source your product before you shut it down" as a universal rule —
plenty of shutdowns don't have a natural open-source path, and plenty of companies that do open
source something still see it languish and die with them. The real lesson is narrower and more
useful: a company's death and its idea's death are two separate events, and the gap between them
is determined almost entirely by what the people in control choose to do in the window between
"we're shutting down" and "we're gone." Facebook used that window well. Most companies don't use it
at all.

## What Founders and Acquirers Should Take From This
- **Advance notice isn't just kindness — it's the mechanism that makes a good ending possible** —
  Parse Server's adoption during the migration window only worked because customers had a full
  year to actually use it
- **Open-sourcing on the way out only works if it's usable, not symbolic** — Parse Server was a
  genuine, deployable alternative, not a token code dump
- **A large acquisition price doesn't determine the ending** — the $85 million Facebook paid for
  Parse says nothing about what happened four years later; the decision to give a year's notice and
  open-source the backend did
- **The company and the idea are not the same asset** — evaluating "did this startup succeed" only
  by whether the company itself survived misses cases exactly like this one
- **Community maintenance can genuinely outlast corporate involvement** — Parse Server has now been
  independently maintained for longer than Parse, Inc. existed as a company

## The Lesson
Most of the videos in this series end with a warning. This one ends with something closer to a
blueprint: what it actually looks like, in specific and dated terms, when a company shuts something
down responsibly — and what can survive as a result.

## Further Reading / Sources
See `sources-log.txt` for the full citation map, including Wikipedia, TechCrunch, VentureBeat, and
the Parse Server GitHub repository.

---

# FAQ (30 Questions)

**1. What was Parse, Inc.?**
A mobile Backend-as-a-Service company founded in 2011, providing cloud data storage, user
authentication, push notifications, and hosted custom code for mobile app developers.

**2. Who founded Parse?**
Ilya Sukhar, James Yu, Tikhon Bernstam, and Kevin Lacker, part of Y Combinator's Summer 2011 batch.

**3. How much did Parse raise before being acquired?**
Reported inconsistently across sources — roughly $7 million to $8.5 million.

**4. Who acquired Parse?**
Facebook, in April 2013.

**5. How much did Facebook pay for Parse?**
A reported ~$85 million, part-cash and part-stock. Facebook never officially disclosed the exact
terms.

**6. Why did Facebook buy Parse?**
It was positioned as Facebook's first-ever paid B2B product, offering backend developer tools.

**7. When did Facebook shut down Parse?**
The hosted Parse.com service shut down on January 28, 2017.

**8. Did Facebook give any warning before shutting Parse down?**
Yes — Facebook announced the shutdown in January 2016, a full year before the actual date.

**9. What happened to Parse's code when it shut down?**
Facebook open-sourced the entire backend as "Parse Server" on the same day it announced the
shutdown.

**10. Is Parse Server still around today?**
Yes — as of 2026, it has 21,407+ GitHub stars and active, ongoing development.

**11. Who maintains Parse Server now?**
An independent community organization, not Facebook, which has had no ongoing involvement since
the 2017 shutdown.

**12. Is Parse Server actually used in production today?**
Yes, based on ongoing GitHub activity and support commitments — though this video doesn't name
specific current companies using it.

**13. What's the difference between Parse.com and Parse Server?**
Parse.com was Facebook's hosted cloud service; Parse Server is the same backend software,
open-sourced so developers can run it on their own infrastructure.

**14. Did most Parse customers actually migrate to Parse Server?**
Yes — it became the default migration path for the large majority of departing Parse.com
customers.

**15. Is this the same story as this channel's "open source killed its own company" video?**
No — that video (a separate package) covers cases where open source competed with and undercut a
paid product. This is the opposite mechanism: the company died for unrelated reasons, and its code
was deliberately open-sourced afterward.

**16. Was Parse's shutdown a failure or a scandal?**
No — this is presented as a responsible, well-executed wind-down, not a failure story.

**17. What happened to Parse's founders afterward?**
Co-founder Ilya Sukhar stayed at Facebook until around 2016, then became a Y Combinator part-time
partner and later a General Partner at Matrix Partners. The other founders' later careers aren't
confirmed in this research.

**18. Is Tikhon Bernstam connected to any other startup this channel has covered?**
Yes — he also co-founded Scribd, the sole surviving company from the YC Summer 2006 batch this
channel fully audited in a separate video.

**19. How many GitHub stars does Parse Server have?**
21,407+, as of this research pass in 2026.

**20. Does Parse Server support current versions of Node.js?**
Yes — documented support for Node.js 18, 20, 22, and 24, with a roadmap through 2028.

**21. Was Facebook's handling of the Parse shutdown unusual?**
Yes — giving a full year's notice and open-sourcing the backend on the same day is notably more
generous than how most acquired platforms are wound down.

**22. What's the core lesson of this video?**
That a company's death and its idea's death are two separate events, and what happens in the gap
between them is determined by the acquirer's choices, not the acquisition price.

**23. Is this a "happy ending" story?**
As close to one as this channel gets — the underlying technology and its community are
demonstrably better off today than the day the company shut down.

**24. How does this compare to this channel's Mailbox video?**
Both are acqui-hire stories where a larger company bought a beloved product and eventually killed
it — but Mailbox was left with no real afterlife, while Parse Server has thrived independently for
almost a decade.

**25. Did Facebook profit from open-sourcing Parse?**
This video doesn't make a claim about Facebook's motives or benefit — it presents the timeline and
outcome as documented.

**26. How long has Parse Server outlived Parse, Inc. as a company?**
As of 2026, roughly nine years since the January 2017 shutdown.

**27. Was Parse profitable as a company before being acquired?**
This video doesn't make a claim about Parse's profitability — that figure wasn't confirmed in
research.

**28. What can other founders learn from how Facebook handled this shutdown?**
That advance notice and a genuine, usable open-source release can determine whether anything
survives a shutdown, regardless of the acquisition price or company size.

**29. Where do you get the information for these videos?**
Public reporting (Wikipedia, TechCrunch, VentureBeat) and the live Parse Server GitHub repository
— all cited on screen and linked in the description and sources log.

**30. What's the main takeaway from this video?**
A company and the idea it built are not the same thing — and how an acquirer handles the ending of
one can determine whether the other survives it, sometimes for far longer than the company itself
ever existed.
