# Understanding of the Problem

This section restates, in our own words, what we understood from the RFP and its supporting materials — so Al Noor can confirm we've read it correctly before any design or build work starts.

## What we understood

Al Noor operates five five-star properties across the UAE. Group Procurement's original instinct was to request a Hotel Management System, but the RFP itself is explicit that this isn't what's being procured here — and the reasoning holds up. Four of five properties already run the same PMS (Opera); the fifth is still being confirmed. That PMS layer reliably captures operational data at each property. The actual breakdown happens **after** the data leaves the PMS: in the business logic Finance and each property apply to it, and in a manual, Excel-based consolidation process that sits entirely outside any property's system.

Two things made this concrete for us:
- **No shared KPI dictionary exists.** When a property and the group office each calculate something like occupancy slightly differently — a different denominator, a different inclusion rule — nobody can quickly tell whether that's a genuine data problem or simply two legitimate definitions in use. The March occupancy discrepancy you describe is a textbook example of this.
- **There's no formal escalation policy.** When a clarification case is still open as the reporting deadline arrives, what happens today is judgment call, not a documented rule.

## What we understood is explicitly *not* the problem

- This is not a data-capture problem. The PMS layer isn't being blamed, and we're not proposing to touch it.
- This is not a request to standardize property operations. Each property's operational independence is intentional, and the RFP is clear that any solution must preserve legitimate property-level differences rather than override them for the sake of group-level tidiness.
- This is not (yet) a guest-facing, booking, or billing problem. Nothing in the RFP's scope touches those systems, and we're not proposing to either.

## What we understood is still open, and why it matters to how we'd approach this

- **Build vs. buy** hasn't been decided internally. We've scoped this response assuming a build engagement, and flagged where that assumption changes the shape of the work (see Proposed Solution and Assumptions, Risks & Dependencies).
- **Executive sign-off on Finance's ownership role** for KPI definitions is still pending. We've treated this as a dependency we need resolved early, not something we can work around.
- **Two further properties' circumstances are still being confirmed** — a fifth property's exact system, and the group's government/tourism reporting obligations property-by-property. We've scoped our proposal around what's confirmed today and treated these as separately-scoped additions once resolved, rather than guessing at them now.

We think this framing is right, but we'd rather have Al Noor correct us now than discover a misunderstanding three weeks into discovery.
