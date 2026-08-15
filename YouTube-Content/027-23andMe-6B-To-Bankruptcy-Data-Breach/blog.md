# Blog Article: 23andMe Hit a $6 Billion Valuation. A Data Breach and a Board Revolt Ended It.

*All figures sourced to CNBC, Fortune, Forbes, Built In SF, Security.org, HIPAA Journal, Dark
Reading, JTA, Forward, Times of Israel, Jerusalem Post, the Office of the Privacy Commissioner of
Canada, Yale Daily News, Al Jazeera, and Caproasia's bankruptcy-filing summary — see
`sources-log.txt` for the full citation map. The 2023 breach is described precisely as a
credential-stuffing attack, not a direct hack of 23andMe's own systems. The Ashkenazi Jewish and
Chinese-ancestry targeting detail is presented factually and soberly, attributed to the specific
reporting that covered it. The $3.5 billion SPAC-deal valuation and the ~$6 billion peak market
value are kept explicitly distinct throughout. The $30 million settlement figure is used as the
primary number; a later-referenced $50 million bankruptcy-court figure is flagged [VERIFY]. Anne
Wojcicki has not been charged with any crime — this is a governance and crisis-management story, not
a fraud story.*

## Introduction
Most stories on this channel follow a familiar shape: a company runs out of money, or a partner
walks away, or a market crashes. 23andMe's story is different. Its core asset wasn't inventory or
software — it was the genetic data of more than 15 million real people. When that asset became a
liability, the company didn't collapse in a straight line. A security incident cascaded into a
governance crisis, and a governance crisis cascaded into bankruptcy — and then, in an ending almost
nothing else on this channel has, the company's own founder bought the core of it back.

## The Founding and the Business
23andMe was founded in 2006 by Anne Wojcicki, Linda Avey, and Paul Cusenza. The business:
direct-to-consumer genetic testing — a mail-in saliva sample returning ancestry and health-risk
information — which later expanded into a research and pharmaceutical data-licensing business built
on top of the company's accumulated genetic database. Over time, more than 15 million people used
the product.

## The Raise and the SPAC
Prior to going public, 23andMe raised "just under $900 million" in total private funding — an
approximate figure, not one precise all-time total, consistent with how this channel treats messy
aggregator numbers — including an $85 million Series F round announced shortly before its SPAC
deal. In February 2021, 23andMe announced it would go public by merging with VG Acquisition Corp.,
a SPAC backed by Sir Richard Branson's Virgin Group, in a deal expected to deliver roughly $984
million in cash at close.

## Going Public: Two Different Numbers
The SPAC deal itself was valued at approximately $3.5 billion when announced. After the merger
closed later in 2021, the stock briefly traded high enough to cross a $6 billion market value — a
separate, higher figure reflecting where the stock actually traded shortly after listing, not the
deal terms themselves. These are two different, both-real numbers, and this article keeps them
distinct throughout: $3.5B is the SPAC deal's announced valuation; $6B is the stock's peak market
value after listing. In June 2021, Anne Wojcicki became a self-made billionaire on paper as a
result.

## What 23andMe Actually Sold
23andMe's product was never just a one-time test result — it was an accumulating genetic database,
made more valuable (and, eventually, more exposed) by features like "DNA Relatives," which shows
customers their genetic connections to other users on the platform. That feature is the reason a
relatively small account breach could expose a much larger population, as the next section
explains.

## The 2023 Breach: How It Actually Happened
Beginning around April 29, 2023, and continuing for about five months, attackers ran a
credential-stuffing attack: reusing usernames and passwords leaked from OTHER, unrelated prior
breaches to log into 23andMe accounts that happened to reuse the same credentials. This was NOT a
breach of 23andMe's own systems or database directly. Approximately 14,000 individual accounts were
directly compromised this way. Because of the "DNA Relatives" family-matching feature described
above, compromising those 14,000 accounts exposed data belonging to approximately 6.9 million total
users. Contributing factors, per subsequent security analysis from HIPAA Journal and Dark Reading:
23andMe did not require two-factor authentication at the time, and its password policy required
only a minimum of eight characters with minimal complexity requirements.

## October 6, 2023: The Reveal
The breach became public on October 6, 2023, after a hacker using the pseudonym "Golem" posted a
database on BreachForums, a cybercrime forum, labeled "Ashkenazi DNA Data of Celebrities," and
separately claimed to possess data belonging to 350,000 users of Chinese heritage, offering both
datasets for sale. This is a real, well-documented, and serious detail, specifically covered by
JTA, Forward, the Times of Israel, and the Jerusalem Post: the breach was marketed by the attacker
as targeting people of Ashkenazi Jewish and Chinese ancestry. It is presented here factually and
soberly, attributed to that reporting, because it is a legitimate and necessary part of the story —
it directly shaped the lawsuits and regulatory response that followed — not an optional detail to
sensationalize or to omit.

## The Settlement and the Regulatory Findings
In September 2024, 23andMe agreed to a $30 million settlement of the resulting class-action
lawsuit, covering the roughly 6.9 million affected users. This is the more widely and consistently
reported figure as of the original settlement. One source, HIPAA Journal, later references a
revised $50 million settlement figure in bankruptcy-court proceedings; this article flags that
later figure as [VERIFY] rather than stating one final settlement number, since a bankruptcy-court
revision has not been independently reconfirmed here. In June 2025, a joint investigation by
Canada's Privacy Commissioner and the UK's Information Commissioner's Office concluded and publicly
criticized 23andMe's security practices in connection with the breach.

## The Board Collapse
Throughout 2024, Anne Wojcicki repeatedly proposed taking 23andMe private, submitting multiple
proposals to the board's special committee. On September 17, 2024, all seven independent directors
resigned from the board on the same day: Roelof Botha, Patrick Chung, Sandra Hernández, Neal Mohan,
Valerie Montgomery Rice, Richard Scheller, and Peter Taylor. Their resignation letter stated
directly that Wojcicki had not delivered "a fully financed, fully diligenced, actionable proposal
that is in the best interests of the non-affiliated shareholders," despite months of engagement.
This is a rare, on-record, board-level statement of no confidence, comparable in strength to other
court-filed or on-record statements this channel has used before, such as James Beriker's statement
in package 023's Munchery story.

## The Layoffs and the Cancer-Research Cut
In November 2024, 23andMe cut more than 200 employees — about 40% of its remaining workforce — and
discontinued its therapeutics/cancer-research division as an emergency cost-cutting measure
following the board exodus.

## Bankruptcy
On March 23–24, 2025, 23andMe filed for Chapter 11 bankruptcy in Delaware. Anne Wojcicki resigned
as CEO effective immediately, remaining only as a board member. The company cited declining stock
value, the fallout from the 2023 breach, the workforce cuts, and the board collapse as converging
causes.

## The Auction: Regeneron vs. TTAM
A two-stage bankruptcy auction followed, contested between Regeneron Pharmaceuticals and Anne
Wojcicki herself, bidding through TTAM Research Institute — a nonprofit she founded specifically to
try to reacquire the company's assets.

## The Twist: What $305 Million Actually Bought
The bankruptcy court approved a $305 million sale to TTAM Research Institute. Anne Wojcicki
ultimately did regain control of the company's core assets, including the genetic data of more than
15 million customers — but only after the public-company structure itself had been wiped out
through bankruptcy. This is a genuinely unusual ending, worth stating explicitly rather than
flattening into a simple "company died" story: the founder ended up back in control of the core
asset — the data — just through a nonprofit vehicle, and for a fraction of the company's SPAC-era
peak valuation.

## The Actual Lesson
23andMe's collapse didn't start with a bankruptcy filing — it started with a security incident that
many companies survive without existential damage. What made it fatal here was the sequence: a
breach that specifically undermined trust in how the company handled its most sensitive asset, a
settlement, a regulatory rebuke, and then a board that ran out of confidence in its own founder's
turnaround plan. The bankruptcy was the last domino, not the first one.

This channel has now covered three SPAC-to-bankruptcy stories, each with a different proximate
cause: Sonder (package 025), where a partner's contract termination triggered the collapse; WeWork
(package 026), where chronic unprofitability plus a second market crash did it; and 23andMe, where
a data breach's fallout compounded into a full board revolt. It is also the only one of the three
where the founder ends the story back in control of a version of the company — a distinct
"founder survives, company doesn't" pattern worth contrasting with package 029 (Ozy Media), where
the founder faces the opposite outcome: an actual criminal conviction. Anne Wojcicki has not been
charged with any crime.

## What Founders and Investors Should Take From This
- **A security incident's real cost is often measured in trust, not just dollars** — the $30
  million settlement was smaller than the governance and reputational fallout that followed it
- **A weak password policy and no mandatory 2FA are structural risks, not minor details** — they
  were the specific contributing factors cited in subsequent security analysis of this breach
- **A board's resignation letter is a rare, citable, on-record signal** — treat it with the same
  evidentiary weight as a court filing
- **Distinguish a deal's announced valuation from its actual peak market value** — 23andMe's $3.5B
  SPAC deal and its $6B peak market value are two different, both-real numbers, and conflating them
  overstates or understates the story depending on which one gets used
- **A bankruptcy doesn't always mean an asset disappears** — 23andMe's core data asset didn't
  vanish, it changed ownership structure, from a public company to a nonprofit controlled by the
  same founder

## The Lesson
23andMe reached a $6 billion peak market value, survived a data breach that specifically targeted
people by ancestry, watched its entire independent board resign in a single day, and filed for
bankruptcy — and its own founder still ended up back in control of the core asset that made the
company valuable in the first place, just through a nonprofit and for a fraction of the original
peak value.

## Further Reading / Sources
See `sources-log.txt` for the full citation map, including links to CNBC, Fortune, Forbes, Built In
SF, Security.org, HIPAA Journal, Dark Reading, JTA, Forward, Times of Israel, Jerusalem Post, the
Office of the Privacy Commissioner of Canada, Yale Daily News, Al Jazeera, and Caproasia. See also
this channel's packages 025 (Sonder) and 026 (WeWork) for the other two SPAC-to-bankruptcy stories,
and package 029 (Ozy Media) for the contrasting founder-conviction outcome.

---

# FAQ (30 Questions)

**1. What was 23andMe?**
A direct-to-consumer genetic testing company, founded in 2006, offering mail-in saliva-sample DNA
kits for ancestry and health-risk information, later expanding into a research and pharma
data-licensing business built on its genetic database.

**2. Who founded 23andMe?**
Anne Wojcicki, Linda Avey, and Paul Cusenza founded the company in 2006.

**3. How much funding did 23andMe raise before going public?**
Just under $900 million in total private funding, including an $85 million Series F round announced
shortly before its SPAC deal — stated as an approximate figure rather than one precise all-time
total.

**4. Did 23andMe go public?**
Yes — in February 2021, it announced a SPAC merger with VG Acquisition Corp., backed by Sir Richard
Branson's Virgin Group, expected to deliver roughly $984 million in cash at close.

**5. What was 23andMe's SPAC deal valued at?**
Approximately $3.5 billion when the deal was announced — a different figure from the company's
later peak market value.

**6. What was 23andMe's peak market value?**
The stock briefly crossed a $6 billion market value shortly after the SPAC merger closed in 2021 —
a separate, higher figure than the $3.5 billion deal-announcement valuation.

**7. Did Anne Wojcicki become a billionaire?**
Yes — in June 2021, she became a self-made billionaire on paper as a result of the SPAC deal.

**8. What caused the 2023 23andMe data breach?**
A credential-stuffing attack: attackers reused usernames and passwords leaked from OTHER,
unrelated prior breaches to log into 23andMe accounts that reused the same credentials. This was
NOT a direct hack of 23andMe's own systems.

**9. How many accounts were directly compromised?**
Approximately 14,000 individual accounts were directly compromised via credential stuffing.

**10. How many people's data was actually exposed?**
Approximately 6.9 million total users, because 23andMe's "DNA Relatives" family-matching feature
exposed genetic-relative connections tied to the compromised accounts.

**11. Did 23andMe require two-factor authentication at the time?**
No — 23andMe did not require two-factor authentication at the time of the breach, and its password
policy required only a minimum of eight characters with minimal complexity requirements.

**12. When did the breach become public?**
October 6, 2023, after a hacker using the pseudonym "Golem" posted a database on BreachForums, a
cybercrime forum.

**13. What did the hacker specifically claim about the stolen data?**
The database was labeled "Ashkenazi DNA Data of Celebrities," and the hacker separately claimed to
possess data belonging to 350,000 users of Chinese heritage, offering both datasets for sale. This
is documented specifically by JTA, Forward, the Times of Israel, and the Jerusalem Post.

**14. Why is the ancestry-targeting detail included in this story?**
Because it is a real, well-documented, and legitimate part of the story — it directly shaped the
resulting lawsuits and regulatory response — presented factually and attributed to the specific
reporting that covered it, not sensationalized.

**15. Did 23andMe settle a lawsuit over the breach?**
Yes — in September 2024, 23andMe agreed to a $30 million settlement covering the roughly 6.9
million affected users. This is the primary, most widely reported figure.

**16. Was there a larger settlement figure mentioned anywhere?**
One source, HIPAA Journal, later references a revised $50 million figure in bankruptcy-court
proceedings. This is flagged as [VERIFY] rather than stated as a confirmed final number.

**17. Did any regulator investigate the breach?**
Yes — a joint investigation by Canada's Privacy Commissioner and the UK's Information
Commissioner's Office concluded in June 2025 and publicly criticized 23andMe's security practices.

**18. Why did 23andMe's board resign?**
On September 17, 2024, all seven independent directors resigned on the same day, stating in their
resignation letter that founder Anne Wojcicki had not delivered "a fully financed, fully
diligenced, actionable proposal that is in the best interests of the non-affiliated shareholders"
for taking the company private, despite months of engagement.

**19. Who were the seven directors who resigned?**
Roelof Botha, Patrick Chung, Sandra Hernández, Neal Mohan, Valerie Montgomery Rice, Richard
Scheller, and Peter Taylor.

**20. What happened after the board resigned?**
In November 2024, 23andMe cut more than 200 employees (about 40% of its remaining workforce) and
discontinued its therapeutics/cancer-research division.

**21. When did 23andMe file for bankruptcy?**
March 23–24, 2025, in Delaware — a Chapter 11 filing.

**22. Did Anne Wojcicki stay CEO after the bankruptcy filing?**
No — she resigned as CEO effective immediately upon the filing, remaining only as a board member.

**23. What caused the bankruptcy, according to the company?**
Declining stock value, the fallout from the 2023 breach, workforce cuts, and the board collapse,
cited as converging causes.

**24. What happened in the bankruptcy auction?**
A two-stage auction was contested between Regeneron Pharmaceuticals and Anne Wojcicki herself,
bidding through TTAM Research Institute, a nonprofit she founded to try to reacquire the company's
assets.

**25. Who won the bankruptcy auction?**
TTAM Research Institute — meaning Anne Wojcicki, through the nonprofit she founded — won with a
bankruptcy-court-approved $305 million sale.

**26. What did the $305 million sale actually include?**
The company's core assets, including the genetic data of more than 15 million customers.

**27. Is the TTAM outcome a "happy ending"?**
It's a genuinely unusual ending worth presenting on its own terms: the founder ended up back in
control of the core asset — the data — just through a nonprofit vehicle, and for a fraction of the
company's SPAC-era peak valuation, after the public company itself was wiped out in bankruptcy.
Readers and viewers may reasonably read it as redemption or as something closer to self-dealing;
both readings are on the table.

**28. Was Anne Wojcicki charged with any crime?**
No — she has not been charged with any crime. This is a governance and crisis-management story, not
a fraud story.

**29. How does this compare to other SPAC-to-bankruptcy stories on this channel?**
This channel has covered two others: Sonder (package 025), triggered by a partner's contract
termination, and WeWork (package 026), driven by chronic unprofitability plus a second market
crash. 23andMe's trigger was a data breach's fallout compounding into a full board revolt — a
different proximate cause each time.

**30. What's the main takeaway from this video?**
23andMe reached a $6 billion peak market value, survived a data breach that specifically targeted
people by ancestry, watched its entire independent board resign in a single day, and filed for
bankruptcy — and its own founder still ended up back in control of the core asset that made the
company valuable, just through a nonprofit and for a fraction of the original peak value.
