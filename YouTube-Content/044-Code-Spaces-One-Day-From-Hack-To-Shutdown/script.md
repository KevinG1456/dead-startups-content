# Script Package

Anchored on Code Spaces — full citations in `sources-log.txt`. THE SINGLE MOST IMPORTANT RULE FOR
THIS SCRIPT: never invent a founder name, funding figure, employee count, or customer count — none
were found anywhere in sourcing. Never state a precise "12 hours" figure for the attack-to-shutdown
timeline — the confirmed dated facts are June 17, 2014 (attack begins) and June 18, 2014 (shutdown
announced); use "the next day" / "within about a day." Keep tone sympathetic to Code Spaces
throughout — this is a victim-of-a-crime story, not a wrongdoing story.

---

## 20 Hooks

1. **(Curiosity)** "This company was hacked on a Tuesday. By Wednesday, it no longer existed."
2. **(Curiosity)** "This company had backups. The hacker deleted those too."
3. **(Fear)** "This is what happens when your backup lives in the exact same place as the thing it's
   supposed to protect."
4. **(Fear)** "No two-factor authentication. One compromised password. One company, gone."
5. **(Story)** "In June 2014, a hacker got into this company's cloud account and asked for money.
   They said no. Here's what happened next."
6. **(Story)** "This company tried to lock the hacker out by changing its password. The hacker was
   already back in before they finished."
7. **(Statistics)** "One DDoS attack. One extortion demand. One company, closed within about a day."
8. **(Statistics)** "Production data: deleted. Backups: also deleted. Same account. Same attacker."
9. **(Mystery)** "Nobody ever found out who did this. Here's exactly what they did anyway."
10. **(Mystery)** "The ransom note came with a Hotmail address. Here's what happened when they
    ignored it."
11. **(Question)** "What actually happens when a company refuses to pay a hacker's ransom?"
12. **(Question)** "Where do your backups actually live — and could the same person delete both?"
13. **(Controversy)** "This company did everything security experts tell you to do when you're
    hacked. It still wasn't enough."
14. **(Controversy)** "This isn't a story about a company that made one big mistake. It's a story
    about one missing checkbox."
15. **(Emotional)** "They refused to be extorted. They lost the company anyway."
16. **(Emotional)** "This is what it looks like to watch your own recovery plan get deleted in real
    time."
17. **(Authority)** "I went through every report on this incident — the extortion note, the AWS
    console logs, the company's own final statement. Here's the real story."
18. **(Authority)** "This is one of the most-cited cloud security case studies in the industry. Most
    people have never heard the full story."
19. **(Challenge)** "Guess how long it took for this company to go from hacked to completely out of
    business."
20. **(Curiosity)** "What does the fastest company death on this entire channel actually look like,
    start to finish?"

**Recommended hook for main cut:** #1 combined with #2.

---

## Complete Viral Script (Main Cut)

**Target length:** 12–14 minutes (the attack, the extortion attempt, the failed recovery, the
deletion, and the shutdown all covered in full, plus the broader lesson)

### Cold Open (0:00–0:15)
- VO: "This company was hacked on a Tuesday. By Wednesday, it no longer existed."
- Visual: a calendar flipping from "TUESDAY" to "WEDNESDAY," with a company logo fading to gray
  underneath
- Pattern Interrupt: hard cut to silence, white text on black: "This isn't a story about a hacker
  being clever. It's a story about where a company kept its backups."

### Hook (0:15–1:00)
- VO: "This is Code Spaces — a small source-code hosting company based in Coventry, England, that
  developers used to store and manage their projects. In June 2014, someone broke into its cloud
  account."
- Open loop: "By the end of this video, you'll understand exactly what the attacker did, why the
  company's own recovery attempt made things worse, and the single specific mistake — one that's
  still extremely common today — that turned a survivable attack into a company-ending one."

### Introduction (1:00–1:40)
- Method statement: reconstructed from HelpNetSecurity, TheHackerNews, Threatpost, eSecurityPlanet,
  CSO Online, and Code Spaces' own final public statement — sourced on screen throughout
- Explicit framing, stated early and plainly: "One honesty note up front: very little is publicly
  known about this company before this incident — no founder name, no funding history, no customer
  count has ever been confirmed anywhere. This video is about what happened during and after the
  attack, which is extremely well documented, not about the company's backstory, which isn't."

### Main Content — The Attack (1:40–5:00)
- **Segment 1 — What Code Spaces Was (1:40–2:10):** a source-code hosting and project-management
  service for development teams — think of it as a place where teams stored their code and tracked
  their work. Visual: simple generic "cloud storage for code" icon graphic.
- **Segment 2 — The DDoS and the Discovery (2:10–3:00):** June 17, 2014, Code Spaces is hit by a
  distributed denial-of-service attack against its servers. While responding, the company discovers
  something worse: messages left inside its own Amazon Web Services control panel. The DDoS wasn't
  the real attack — it was cover. Visual: "JUNE 17, 2014 — THE ATTACK BEGINS" title card.
- **Segment 3 — The Ransom (3:00–3:45):** the attacker had gained access to Code Spaces' AWS EC2
  control panel and left extortion demands, including a Hotmail contact address, demanding payment
  to stop the DDoS attack. Visual: stylized (non-identifying) "ransom note" graphic with the demand
  text.
- **Segment 4 — The Company Says No (3:45–4:30):** Code Spaces refused to pay. Instead, the company
  tried to take back control the obvious way: changing the account's passwords. Visual: "DEMAND:
  DECLINED" stamp card.
- **Segment 5 — The Trap (4:30–5:00):** the attacker had anticipated exactly this move. They had
  already created extra backup administrator logins into the AWS console — so when Code Spaces
  changed its main password, the attacker simply used one of the backup logins to get right back in.
  Visual: a "door" graphic being locked, then a second hidden door opening behind it.

### Main Content — The Deletion (5:00–8:00)
- **Segment 6 — The Deletion Begins (5:00–6:00):** back inside, the attacker began deleting
  artifacts across the account: EBS snapshots, S3 storage buckets, Amazon Machine Images, EBS
  instances, and multiple machine instances. Visual: a file-tree graphic collapsing/disappearing
  branch by branch.
- **Segment 7 — The Detail That Changes Everything (6:00–7:00):** here's the detail that turned a
  bad day into a company-ending one — Code Spaces kept its backups in the SAME AWS account as its
  production data. There was no separate, isolated copy anywhere else. When the attacker deleted the
  account's contents, they deleted the backups in the exact same sweep. On-screen framing card: "A
  backup that can be deleted by the same person, at the same time, as the original isn't really a
  backup." Visual: two identical folder icons labeled "PRODUCTION" and "BACKUP" — both dissolving
  simultaneously.
- **Segment 8 — The Missing Setting (7:00–8:00):** Code Spaces later confirmed, via its own Twitter
  account, that the AWS account had no two-factor authentication enabled — the best-sourced
  explanation available for how the attacker got in with just a compromised username and password in
  the first place. Visual: "NO TWO-FACTOR AUTHENTICATION" title card with a simple unchecked
  checkbox graphic.

### Main Content — The Ending (8:00–10:30)
- **Segment 9 — What Was Actually Lost (8:00–8:45):** customer source code, project data, and
  configuration files were permanently deleted, along with the company's own backups. With
  infrastructure and backups gone, there was no way to rebuild. Visual: "PRODUCTION DATA: GONE.
  BACKUPS: ALSO GONE." title card.
- **Segment 10 — The Statement (8:45–9:45):** June 18, 2014 — the day after the attack began — Code
  Spaces posted a statement on its own website: "Code Spaces will not be able to operate beyond this
  point, the cost of resolving this issue to date and the expected cost of refunding customers who
  have been left without the service they paid for will put Code Spaces in an irreversible position
  both financially and in terms of ongoing credibility." The company said it would spend its
  remaining resources helping customers export whatever data could still be recovered. Visual: quote
  card, company's actual statement text on screen, attributed.
- **Segment 11 — The Attacker, Never Found (9:45–10:30):** Code Spaces' own statement specified that
  the attacker was "unauthorized" and, as far as the company could tell, had no connection to any
  current or former employee. No perpetrator was ever identified. Visual: "NO PERPETRATOR EVER
  IDENTIFIED" title card.
- Mid-video CTA (~10:00): "This channel usually covers companies that ran out of money or lost a
  market. This is the fastest death on the entire channel — and the cause fits in one sentence.
  Subscribe for a new autopsy every week."

### The Actual Lesson (10:30–12:00)
- Plain-language comparison: Code Spaces did the thing security guidance tells you to do when you're
  extorted — it refused to pay. That was the right call. It just wasn't enough, because the deeper
  problem had already been built into the account architecture months or years earlier: one set of
  credentials with no second factor, and one account holding both the only copy of the product and
  the only copy meant to protect it.
- The core lesson, stated directly: a backup is only a backup if the person who can destroy your
  original data can't also destroy it. Co-locating backups with production, and skipping two-factor
  authentication on the account that controls both, are still extremely common mistakes today — this
  isn't a 2014 problem, it's a 2026 problem wearing a 2014 case study.
- Visual: full-arc timeline graphic — DDoS begins (Jun 17, morning) → console access discovered →
  ransom demand → password change attempted → attacker re-enters via backup login → mass deletion of
  production AND backups → shutdown statement posted (Jun 18) → no perpetrator ever found.

### Final CTA + Outro (12:00–13:00)
- VO: recap the one-sentence lesson — a backup that lives next to the thing it's protecting isn't a
  backup, it's just a second target
- "Subscribe — I'm building a full library of these, and this is the fastest one yet: a company that
  went from a normal Tuesday to fully closed by Wednesday"
- Engagement prompt: "If you run any part of a company's infrastructure — is your backup actually
  isolated from your production account, or one compromised password away from being deleted right
  alongside it? Tell me in the comments."
- End screen: most recent autopsy + subscribe

---

## Alternative Scripts

### Script Version A — Technical / DevOps-Forward Style
Opens directly on the AWS console mechanics (the backup admin logins, the deletion sequence) as the
core narrative spine, treating the human/company-death framing as the emotional close rather than the
opening hook. Denser on the specific AWS services affected (EBS, S3, AMIs). Strongest fit for
repurposing into a dedicated DevOps/cloud-security audience cut.

### Script Version B — Narrative / Documentary Style
Opens on the ransom note itself — the Hotmail address, the demand — before cutting hard to the June
18 shutdown statement, then rewinding to fill in the full sequence in between. Slower pacing, holds
the "backups were in the same account" reveal until Segment 7, resolving on the "no perpetrator was
ever found" beat as the closing note of unresolved tension.

### Script Version C — Fast-Cut / Listicle Style
Structured as "one bad Tuesday, five mistakes" leading into rapid-fire beats: DDoS as cover, console
access, ransom ignored, password change, backup-login re-entry, mass deletion, no MFA, no isolated
backup, shutdown statement, no perpetrator found — landing on the "backups in the same account"
lesson as the final, clarifying beat. Strong Shorts-extraction potential, especially the "they had
backups, the hacker deleted those too" beat and the "no perpetrator was ever found" close.

---

## Audience Retention Optimization
- **Drop-off risk:** the technical AWS-mechanics segment (5:00–6:00) if the specific service names
  (EBS, S3, AMIs) feel like unexplained jargon to a general audience
- **Fix:** translate each AWS term into plain language immediately on screen the first time it's
  used ("EBS snapshots — essentially saved copies of a server's hard drive")
- **Faster pacing opportunity:** trim the general "what Code Spaces was" segment if early-retention
  data shows the audience doesn't need company-category context before the attack begins
- **Curiosity increase opportunity:** tease the "the backup didn't save them" reveal even more
  explicitly in the cold open if drop-off appears before Segment 7 (6:00)
- **Recommended visual change:** keep a small running timeline counter visible from Segment 2 onward
  ("DAY 1: MORNING" → "DAY 1: AFTERNOON" → "DAY 2") so the speed of the collapse stays viscerally
  present throughout, without ever displaying an unverified precise hour count

---

## Chapters / Timestamps
- 00:00 Cold Open
- 00:15 The Real Question
- 01:00 How This Video Is Built (Sources + Honesty Note)
- 01:40 What Code Spaces Was
- 02:10 The DDoS and the Discovery
- 03:00 The Ransom
- 03:45 The Company Says No
- 04:30 The Trap
- 05:00 The Deletion Begins
- 06:00 The Detail That Changes Everything
- 07:00 The Missing Setting
- 08:00 What Was Actually Lost
- 08:45 The Statement
- 09:45 The Attacker, Never Found
- 10:00 Mid-Video: The Fastest Death on This Channel
- 10:30 The Actual Lesson
- 12:00 What's Next
