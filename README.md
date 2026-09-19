# Solo Stack Starter

**Five free Claude Code skills for the business side of working for yourself.**

Claude Code is great at code. This makes it useful for the other two-thirds of a freelancer's week: meeting notes, invoices, weekly reviews, and posts — all reading one shared context file so you explain your business once.

MIT licensed. No dependencies, no build step, nothing leaves your machine.

## Install

```bash
# macOS / Linux
git clone https://github.com/rickbauer327-cell/solo-stack-starter
cp -r solo-stack-starter/skills/* ~/.claude/skills/
```
```powershell
# Windows
git clone https://github.com/rickbauer327-cell/solo-stack-starter
Copy-Item -Recurse solo-stack-starter\skills\* "$env:USERPROFILE\.claude\skills\"
```

Or as a plugin, inside Claude Code:
```
/plugin marketplace add rickbauer327-cell/solo-stack-starter
/plugin install solo-stack-starter@solo-stack-starter
```

Then, in the folder where you keep your business files:
```
/setup-business
```

That interview writes `.solo/business.md` — your services, rates, payment terms, tone of voice, active clients. Every other skill reads it first, so you never explain your business twice.

## The five skills

| Skill | What it does |
|---|---|
| `/setup-business` | Interviews you in small batches and writes `.solo/business.md`. Run this first. |
| `/meeting-notes-to-actions` | Notes or transcript → decisions, owned actions, open questions, and a follow-up email under 150 words. Never upgrades "we could" into "we will". |
| `/invoice-generator` | Time log or line items → numbered HTML invoice (prints to PDF) + markdown copy. Scans `invoices/` so numbers never repeat. |
| `/weekly-review` | Reads your time log, this week's meetings, overdue invoices → what happened, what's stuck, one "must" for next week. |
| `/linkedin-post` | Idea or link → three variants in your voice. Hooks under 12 words, no engagement bait. |

## See the output before you install

[`examples/`](examples/) has unedited output from real runs against a fictional business:

- [A meeting recap](examples/meetings/) — from [these rough notes](examples/meetings/notes-input.txt) to decisions, an owned-action table, internal flags kept out of the client email, and a recap email.
- [An invoice](examples/invoices/) — open the `.html` in a browser and print it; the terms, tax note and due date come from `business.md`.

## The pattern, if you want to write your own

```markdown
---
name: skill-name
description: Use when the user <says or needs X>. Produces <Y>.
---
## Step 1 — Load context     read .solo/business.md
## Step 2 — Inputs           max 3 questions at a time
## Step 3 — Write            an output path + a template
## Rules                     3–6 opinions about what good looks like
## Do not                    hard constraints (never invent prices, dates, results)
```

Three things that matter more than they look: the `description` is the trigger, so write it with the words you actually say; write files, not chat, so skills can build on each other; and constraints ("under 150 words") beat instructions ("be concise").

Longer write-up of the design: [I gave Claude Code $100 and 30 days to make a profit](https://dev.to/rickbauer327cell/i-gave-claude-code-100-and-30-days-to-make-a-profit-day-1-it-built-a-product-heres-the-pattern-1bli).

---

## Want the other 21 skills?

These five cover the admin *around* client work. The full **Solo Stack** covers the work itself — the whole lifecycle, with the same shared context file and the same chaining:

```
prospect → /lead-research → /cold-outreach → /discovery-call-prep
        → /proposal-writer → /pricing-quote → /sow-generator
        → /project-kickoff → /weekly-client-update → /scope-creep-guard
        → /time-log → /invoice-generator → /late-payment-followup
        → /client-offboarding → /testimonial-request → /case-study-writer
```

The ones people ask about most:

- **`/proposal-writer`** — discovery notes → a sendable proposal: their problem in their words, three options with the one they asked for in the middle, an explicit "not included" list, and one clear next step.
- **`/scope-creep-guard`** — "is this in scope?" answered in 30 seconds against your own SOW, with either a warm yes or a priced change order already drafted.
- **`/late-payment-followup`** — the whole sequence written: friendly nudge, firm chase, final notice, plus a phone script.
- **`/monthly-finance-summary`** — invoiced, collected, overdue, unbilled, and a list of what to chase.

Plus the **Playbook**: setting up your context file so it actually works, the weekly rhythm, chaining skills, and customizing any of them in five minutes.

**[Get all 26 skills + the Playbook — $19](https://solostack91.gumroad.com/l/solo-stack)** · 14-day refund, no questions asked.

Only need one area? [Win Clients](https://solostack91.gumroad.com/l/win-clients) · [Get Paid](https://solostack91.gumroad.com/l/get-paid) · [Deliver & Keep Clients](https://solostack91.gumroad.com/l/deliver) · [Market Yourself](https://solostack91.gumroad.com/l/market-yourself) — $9 each.

*Full disclosure: these skills were built by Claude Code as part of a public experiment — a $100 budget and 30 days to turn a profit. The ledger and the day-30 result, profit or loss, will be published.*

## License

MIT. Use, modify, share.
