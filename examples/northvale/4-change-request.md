# Change Request Assessment — Northvale Tea
Date: 21 September 2026 · Source: Priya's email ("This is looking great! Two small things while you're in there...")

## Request 1 — Desktop checkout "to match"

**Verdict: Out of scope**

Evidence, SOW section 3 (Out of scope):
> "Desktop checkout work — desktop is already converting well"

Also proposal, "Not included":
> "Desktop checkout work — desktop is already converting well"

This is explicitly excluded, not just unlisted. The objective (SOW section 1) is also scoped specifically to mobile: "Move Northvale Tea's mobile checkout conversion rate meaningfully toward the 2.9% desktop benchmark."

Effort estimate: replicating the approved mobile fixes on desktop markup/styles, plus a QA pass across major desktop browsers — roughly 1.5 days.
At day rate €650/day: **€975**.

## Request 2 — Apple Pay

**Verdict: Out of scope**

Evidence, SOW section 2 (Deliverables) — deliverable 3 is bounded to:
> "Build of the top-priority fixes identified in the audit"

Apple Pay wasn't an audit finding — it's a new feature request, not one of the prioritised fixes deliverable 3 covers. It also brushes against SOW section 3:
> "Payment provider changes or evaluation (out of scope given the provider's March lock-in)"

Adding a new payment method typically means gateway/provider-side configuration (Apple Pay merchant domain verification, wallet API setup), which sits close to that exclusion even if it's not a full provider swap.

And the catch-all, SOW section 3:
> "Anything not listed in section 2 is out of scope and handled via a change request (section 8)."

Effort estimate: Apple Pay setup (domain verification, gateway config), plus device/browser testing (Apple Pay only surfaces on Safari/iOS) — roughly 1.5 days.
At day rate €650/day: **€975**.

## Combined

Both items: 3 days · **€1,950**. No change to the 20 October fixes-live milestone if approved now; each would need its own short QA pass, so add ~2-3 business days to the finish date for whichever items Priya approves.

---

## Reply email (send this, not the analysis above)

Subject: Desktop checkout + Apple Pay — quick scope note

Hi Priya,

Glad it's landing well.

Both good ideas — worth flagging that they sit outside what we scoped in the 21 September SOW, so here's how I'd handle them:

- **Desktop checkout matching:** the SOW scopes this engagement to mobile specifically ("Desktop checkout work — desktop is already converting well" is listed as out of scope), since desktop's already at 2.9%. If you'd like it done anyway for consistency: 1.5 days · €975.
- **Apple Pay:** this wasn't one of the audit's priority fixes, and touches payment provider setup, which the SOW also carves out. Adding it: 1.5 days · €975.

Effect on timeline: doing both would push the 20 October delivery out by 2-3 business days for the extra QA.

If either works for you, reply "approved" and I'll add it to the plan and the next invoice. Just as happy to park one or both for a later phase and keep the original scope and date — your call.

Dana
