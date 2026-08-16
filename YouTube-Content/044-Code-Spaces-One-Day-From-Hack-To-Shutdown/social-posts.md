# Social Posts

## X / Twitter Thread

1/ This company was hacked on a Tuesday. By Wednesday, it no longer existed.

Here's exactly what happened — and the one mistake, still extremely common today, that turned a
survivable attack into a company-ending one. 🧵

2/ June 17, 2014. Code Spaces, a small source-code hosting company, gets hit by a DDoS attack.

While responding, they find something worse: someone has console access to their AWS account.

3/ The attacker leaves a ransom demand. Pay up, or the DDoS continues.

Code Spaces says no. They try to lock the attacker out by changing their passwords.

4/ It doesn't work. The attacker had already planted backup admin logins into the account.

They get back in — and start deleting everything.

5/ Here's the detail that changes everything: Code Spaces kept its backups in the SAME account as
its production data.

When the attacker deleted the account, they deleted the backups too. There was nothing left to
restore from.

6/ Company also later admitted: no two-factor authentication on the account. Best-sourced
explanation for how the attacker got in with just a stolen password in the first place.

7/ June 18, 2014 — the next day — Code Spaces posts a statement: they're shutting down for good. The
damage, financial and reputational, is irreversible.

No perpetrator was ever identified.

8/ The lesson isn't "get better security." It's more specific than that: a backup that the same
attacker can delete at the same time as your original data isn't a backup. It's a second target.

Full breakdown on the channel — link below.

## LinkedIn Post

A company was hacked on a Tuesday. By Wednesday, it no longer existed.

I just published a full breakdown of the Code Spaces incident — one of the most-cited cloud security
case studies in the industry, and one I think a lot of founders and operators outside pure security/
DevOps circles have never heard the full story of.

The short version: a hacker got console access to the company's AWS account, demanded a ransom, and
when the company refused and tried to lock them out, the attacker got back in through a backdoor
they'd already planted — and deleted everything. Including the backups. Because the backups lived in
the same account as the data they were supposed to protect.

The company did the right thing by refusing to pay. It wasn't enough, because the real vulnerability
had been built into the account architecture long before the attack ever started.

If you run any part of your company's infrastructure, this is worth ten minutes. Full video linked
in the comments.

## Instagram Caption
A hacker demanded a ransom. This company said no.

They still lost everything — because their backups lived in the same place as their data.

Full story on the channel. 🔗 in bio.

#CodeSpaces #CyberSecurity #StartupFailure #CloudSecurity
