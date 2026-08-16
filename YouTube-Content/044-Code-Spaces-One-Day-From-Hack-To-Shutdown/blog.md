# Blog Article

## Title: Hacked on a Tuesday. Out of Business by Wednesday. What Actually Killed Code Spaces.

In June 2014, a small UK-based company called Code Spaces went from operating normally to
completely shut down in about a day. Not "struggling." Not "restructuring." Gone — its own website
carrying a final statement announcing the company could no longer operate.

The cause fits in a single sentence, and it's a mistake that remains extremely common today, over a
decade later: the company's backups lived in the same place as the data they were supposed to
protect.

**A note on what we do and don't know about this company.** Code Spaces was a source-code hosting
and project-collaboration service based in Coventry, UK — that much is confirmed. Beyond that, very
little is publicly documented: no founder name, no founding year, no funding history, and no
customer count appear anywhere in the public record. Nearly everything ever written about this
company was written after the incident described below. This article, like the video it accompanies,
covers what's genuinely well documented — the attack itself — rather than guessing at a backstory
nobody has ever published.

### The attack that wasn't what it looked like

On June 17, 2014, Code Spaces was hit by a distributed denial-of-service (DDoS) attack against its
servers. That alone wasn't unusual — DDoS attacks against online services were, and remain, common.

What made this one different is what the company discovered while responding: messages left inside
its own Amazon Web Services (AWS) EC2 control panel. The DDoS attack wasn't the point. It was cover.
Someone had gained actual administrative access to the account that ran the company's infrastructure.

### The ransom

The intruder left extortion demands, including a contact address at Hotmail, requesting a payment to
stop the DDoS attack. Code Spaces refused to pay.

Refusing to pay an extortion demand is, by every standard piece of security guidance, the right
call. Paying doesn't guarantee an attacker stops, and it confirms the target is willing to pay —
inviting more attempts. Code Spaces did the thing it was supposed to do.

### The recovery attempt that made things worse

Instead of paying, the company tried to retake control the obvious way: changing the account's
passwords to lock the attacker out.

The attacker had anticipated exactly this. Before the company could act, the intruder had already
created additional backup administrator logins into the AWS console. When Code Spaces changed its
main credentials, the attacker simply used one of those backup logins to get straight back in.

### The deletion

Back inside the account, the attacker began deleting artifacts, seemingly as the company continued
trying to respond: EBS (Elastic Block Store) snapshots, S3 storage buckets, Amazon Machine Images
(AMIs), EBS instances, and multiple machine instances.

In plain terms: this wasn't a narrow, surgical attack on one system. It was a broad sweep across
essentially everything the account controlled.

### The detail that turned a bad day into a company-ending one

Here is the single most important fact in this entire story: Code Spaces kept its backups in the
same AWS account as its production data.

There was no separate, isolated copy anywhere else — no second account, no offline archive, no
independently access-gated storage. When the attacker deleted the account's contents, they deleted
the backups in the exact same sweep as the production data they were meant to protect.

A backup that can be destroyed by the same person, using the same access, at the same time as the
original isn't functioning as a backup. It's just a second copy of the same target.

Company representatives later confirmed, via the company's own Twitter account, that the AWS account
had no two-factor authentication (2FA) enabled. The best-sourced explanation for how the attacker
gained initial access in the first place is a compromised username and password — a single point of
failure that 2FA is specifically designed to prevent.

### The end

On June 18, 2014 — the day after the attack began — Code Spaces posted a statement on its own
website:

> "Code Spaces will not be able to operate beyond this point, the cost of resolving this issue to
> date and the expected cost of refunding customers who have been left without the service they
> paid for will put Code Spaces in an irreversible position both financially and in terms of ongoing
> credibility."

The company said it would use whatever resources remained to help customers export any data that
could still be recovered. Customer source code, project data, and configuration files had been
permanently deleted, alongside the company's own backups. There was no way to rebuild.

No perpetrator was ever identified. Code Spaces' own statement specified that the intruder was
unauthorized and, as far as the company could determine, had no connection to any current or former
employee.

### The actual lesson

It would be easy to read this as a simple "get better security" story, but that undersells what
actually happened. Code Spaces did the specific thing security guidance recommends when facing
extortion — it said no. That decision was correct, and it still wasn't enough, because the real
vulnerability had been built into the account architecture long before the attacker ever showed up:
one set of credentials with no second factor standing between a compromised password and the entire
company, and one account holding both the only copy of the product and the only copy meant to
protect it.

Co-located backups and missing multi-factor authentication remain two of the most common
misconfigurations in cloud infrastructure today — this isn't a relic of 2014's relative cloud
immaturity. If anything, more companies run entirely on cloud infrastructure now than did in 2014,
which makes the lesson more relevant, not less.

The question worth asking about your own infrastructure isn't "do we have backups." It's: if the
credentials protecting our production environment were compromised right now, could the same
attacker also reach and delete our backups? If the honest answer is yes, the backup isn't doing the
job a backup is supposed to do.

---

*Sources: HelpNetSecurity, TheHackerNews, Threatpost, Darknet.org.uk, eSecurityPlanet, CSO Online,
DataBreaches.Net, breaches.cloud, and Code Spaces' own final public statement. Full citation list
available in this video's production notes.*
