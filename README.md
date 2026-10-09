# Momentum - AI Sales Team for a Mercedes-Benz Salesperson

Five Claude agents (in `.claude/agents/`) focused on repeat and referral business.

| Agent | Use it to |
|---|---|
| prospector | Rank who to contact (lease-ends, upgrades, referral candidates) |
| outreach-writer | Draft texts/emails/call openers in your voice |
| follow-up | Know who is due and draft the next touch |
| deal-manager | Update deals, prep appointments, handle objections |
| daily-briefing | Morning plan and end-of-day recap |

## Setup
1. Fill in `context/profile.md`.
2. Export your client list from the CRM (UDC) as CSV into `data/` (gitignored - never committed). Or start with `templates/pipeline-tracker.csv`.
3. In Claude Code, ask e.g. "Run the prospector on data/clients.csv" or "daily-briefing".

Agents only draft; you review and send. Rules in `.claude/agents/_shared-rules.md`.
