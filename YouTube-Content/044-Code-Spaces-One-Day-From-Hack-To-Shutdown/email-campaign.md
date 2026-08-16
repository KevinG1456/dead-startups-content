# Email Campaign

## Email 1 — Launch Announcement
**Subject:** They were hacked on a Tuesday. By Wednesday, they were gone.
**Preview text:** The backup didn't save them. Here's why.

Body:
This week's autopsy is the fastest one on the whole channel.

In June 2014, a small company called Code Spaces got hit with a DDoS attack — which turned out to be
cover for something worse. Someone had gotten into their AWS account and left a ransom demand.

They said no. They tried to lock the attacker out. It didn't work — and by the next day, the company
had announced it was shutting down for good.

The reason is one sentence long, and it's still an extremely common mistake today: their backups
lived in the same account as their production data. When the attacker deleted the account, they
deleted the backups too.

Watch the full breakdown: [LINK]

## Email 2 — Mid-Week Follow-Up (sent to non-openers)
**Subject:** The cloud security case study most founders have never heard
**Preview text:** One missing setting. One dead company.

Body:
If you missed it — this week I covered one of the most-cited cloud security incidents in the
industry, and I don't think most people outside security/DevOps circles have ever heard the full
story.

Short version: a company refused to pay a hacker's ransom (the right call), tried to lock them out,
and lost everything anyway — because the real vulnerability had already been built into their setup
long before the attack: no two-factor authentication, and backups stored in the same place as
production.

Ten minutes, full breakdown: [LINK]

## Email 3 — Engagement / Discussion Prompt
**Subject:** A question for anyone who runs infrastructure
**Preview text:** Could the same compromised password reach both your data and your backup?

Body:
After this week's video on the Code Spaces shutdown, I got a lot of replies from people in DevOps/
engineering roles with their own near-miss stories — accounts that almost had exactly this happen.

If you haven't watched yet, it's worth the ten minutes, especially if you're not 100% sure your
backups are actually isolated from your production account: [LINK]

Reply and tell me — have you ever had a close call like this?
