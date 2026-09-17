# Review Ask Setup

**Portfolio project** by [Travis Hambrick](https://github.com/travisrafehambrick-max)

A simple, done-for-you style automation for local service businesses: after a job goes well, the customer gets a short text with a Google review link. Happy customers go to Google. Unhappy ones reply to the owner first.

This is **not** inventing a new product category (tools like Podium, Birdeye, NiceJob, and Housecall Pro already exist). It is a **lightweight setup** owners will actually use without buying another expensive dashboard.

---

## Problem

Local shops do good work but forget to ask for reviews. Competitors with more Google reviews show up first in Maps — even when the work quality is worse.

## What I built / demonstrated

1. Pulled a real **Google Business Profile review link** (`Get more reviews` → copy link).
2. Wrote a short customer message (owner voice, happy path + unhappy path).
3. **Self-tested**: texted the message to myself, tapped the link, confirmed the Google review form opens.

That is the core customer experience. Automation (auto-send after job close) is the next layer.

## How it works (manual → automated)

```
Job finished
    → send SMS/email with review link
    → happy customer leaves Google review
    → unhappy customer replies to owner (stays private)
```

**Manual today:** owner (or Travis) sends the template after each job.  
**Automated later:** trigger from their scheduling/CRM tool or a simple button/workflow (n8n, etc.).

## Message template

See [`templates/customer-message.txt`](templates/customer-message.txt).

## Who it’s for

Phone/field businesses with **good reviews but not many of them**: HVAC, plumbing, electrical, lawn, cleaning, auto, salon, etc.

**Buyer question:**  
“When a job goes well, do you text people a Google review link — or does it just not happen?”

## What’s in this repo

| File | Purpose |
|------|--------|
| `README.md` | Project story for resume / employers |
| `templates/customer-message.txt` | Copy-paste SMS/email |
| `docs/setup-checklist.md` | Steps to set this up for a real business |

## Resume one-liner

> Designed and self-tested a lightweight Google review-request flow for local service businesses (message template + GBP review link + customer happy/unhappy path).

## Status

- [x] Review link + message self-test
- [ ] First live setup for a real local business
- [ ] Optional auto-send after job completion

## License

Personal portfolio / learning project. Not affiliated with Google or any review-SaaS vendor.
