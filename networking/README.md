# Networking — Target Tracking

This folder is the "CRM" for people **outside Jason's network** that we want to
reach for the Anthropic Head of Sales goal (and adjacent opportunities).

Everything in here is **manually captured public/Sales-Nav-visible info** —
LinkedIn Premium is the research tool; this repo is the structured record.
No scraping; just notes a salesperson would normally keep in a spreadsheet
or Notion, but in version control so we can diff & track over time.

## Layout

```
networking/
├── README.md                       — this file
├── target_list.md                  — running roll-up of all targets w/ status
├── outreach_log.md                 — chronological log of every touch
├── targets/                        — one Markdown file per person
│   ├── _template.md                — copy this when adding a new target
│   └── <firstname-lastname>.md
└── inbound/                        — people who reach out TO Jason
    └── <firstname-lastname>.md
```

## Workflow

1. **Find** a target in LinkedIn Sales Navigator (or Apollo / Clay / company site / podcast / X).
2. **Copy** `targets/_template.md` → `targets/firstname-lastname.md`. Fill it in
   with what's publicly visible. Note mutual connections, hooks, anything they've
   posted recently.
3. **Decide** the outreach angle (warm intro vs. cold InMail vs. comment-on-post
   vs. event). Capture the planned ask + draft message in the file.
4. **Log** every touch (InMail sent, reply, intro made, call booked) in
   `outreach_log.md` with a date.
5. **Update** `target_list.md` with the new status (`prospect → contacted →
   replied → meeting → referral → applied`).

## Bulk enrichment

When we have a list of names (e.g., "everyone on the Anthropic GTM team"),
use one of these to pull public role/email data into a CSV, then convert
to per-target files:

- **Apollo.io** — free tier gives credits; has Anthropic indexed; CSV export.
- **Clay.com** — workflow tool; great for enriching a CSV with public data.
- **LinkedIn Sales Navigator → Lead List → Export** (Premium feature you already have).

## Privacy note

This folder will contain real names and notes. Keep the repo **private**.
Don't push contact info (emails, phone numbers) to a public repo if this
ever flips public — put those in a gitignored `*.private.md` instead.
