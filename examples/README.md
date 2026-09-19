# Examples

Unedited output from real runs against the fictional business in [`.solo/business.md`](.solo/business.md). Nothing here was touched by hand.

| Input | Skill | Output |
|---|---|---|
| [rough call notes](meetings/notes-input.txt) | `/meeting-notes-to-actions` | [**rendered recap**](meetings/2026-09-15-acme-coffee-checkout-redesign.html) · [markdown the skill wrote](meetings/2026-09-15-acme-coffee-checkout-redesign.md) |
| "Invoice Acme Coffee for the 50% deposit, project value 2600 EUR" | `/invoice-generator` | [**invoice**](invoices/INV-0001-acme-coffee.html) · [markdown copy](invoices/INV-0001-acme-coffee.md) |

Open either `.html` in a browser. Both print cleanly to PDF — the invoice is what a client receives.

**What to look for in the recap**, because it is the whole point:

- Sam's "maybe a loyalty programme later, budget isn't approved" became an internal **flag**, not a decision.
- An action with no stated date reads **(no date set)** instead of an invented one.
- The flags never appear in the client-facing email.
