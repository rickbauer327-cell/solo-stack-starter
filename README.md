# Solo Stack Starter

**Five free Claude Code skills for the business side of working for yourself.**

Claude Code is great at code. This makes it useful for the other two-thirds of a freelancer's week: meeting notes, invoices, weekly reviews, and posts — all reading one shared context file so you explain your business once.

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

Then in the folder where you keep your business files:
```
/setup-business
```

## The five skills

| Skill | What it does |
|---|---|
| `/setup-business` | Interviews you (in small batches) and writes `.solo/business.md` — services, rates, terms, tone, clients. Every other skill reads it first. |
| `/meeting-notes-to-actions` | Notes or transcript → decisions, owned actions, open questions, and a follow-up email under 150 words. Never upgrades "we could" into "we will". |
| `/invoice-generator` | Time log or line items → numbered HTML invoice (prints to PDF) + markdown copy. Scans `invoices/` so numbers never repeat. |
| `/weekly-review` | Reads your time log, this week's meetings, overdue invoices → what happened, what's stuck, one "must" for next week. |
| `/linkedin-post` | Idea or link → three variants in your voice. Hooks under 12 words, no engagement bait. |

## The pattern

Every skill here follows the same shape, and you can use it for your own:

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

## The full pack

Solo Stack has 26 skills covering the whole client lifecycle — lead research, cold outreach, discovery-call prep, proposals, pricing, SOW, kickoff, weekly client updates, scope-creep guard, late-payment sequence, monthly finance summary, case studies, testimonials, a one-file portfolio site, inbox triage, SOPs, decision memos — plus a playbook on chaining and customizing them.

→ **[Get Solo Stack on Gumroad](https://solostack91.gumroad.com/l/solo-stack)** — $19 during launch.

## License

MIT. Use, modify, share.
