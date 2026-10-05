# Hotel Management System (PMS/HMS) Vendor Landscape

**Purpose:** Build a realistic shortlist-style view of the vendor market this RFP would actually go to, so the eventual RFP distribution list and evaluation criteria reflect real market options rather than generic placeholders. This is preliminary desk research, not a vendor recommendation — a real RFP would issue an open or targeted call and let vendors self-qualify.

**Source caveat:** Several sources below are vendor-comparison/marketing sites, not vendor-neutral analyst reports. Claims are reported as "vendor positions itself as..." rather than independently verified facts, and should be re-validated via vendor RFI responses before being relied on for a real decision. Full citations in [`sources.md`](sources.md).

## Enterprise-tier (large chains, luxury, multi-property)

| Vendor | Positioning | Noted strengths | Noted weaknesses / considerations |
|---|---|---|---|
| **Oracle OPERA (Cloud)** | Positioned for large global hotel chains, luxury properties, and international hospitality groups[^1] | Long-standing "global enterprise standard" with deep multi-property/chain functionality[^1]; widely deployed in luxury brands | Reported as expensive, with long implementation cycles; legacy-architecture concerns raised in comparison sources[^1] |
| **Infor HMS** | Positioned for large hotel chains/groups already inside the Infor ERP ecosystem[^1] | Strong if already on Infor ERP; multi-property dashboards[^1] | Tied to the Infor ecosystem, which can limit flexibility for groups wanting a standalone best-of-breed PMS[^1] |
| **Shiji (Infrasys / Shiji Enterprise Platform)** | Enterprise hospitality platform, positioned as an alternative to Oracle OPERA for hotel groups[^2] | Frequently cited as a modern cloud alternative to legacy enterprise PMS | Needs direct vendor validation — not independently confirmed in this research pass |
| **protel PMS (by Planet)** | Enterprise/multi-property PMS, part of the Planet payments/hospitality group | Positioned as an OPERA alternative for chains | Needs direct vendor validation |

## Mid-market / cloud-native (noted for completeness — may not fit a five-star brand standard without validation)

- Cloudbeds, RMS Cloud, StayNTouch, Mews, IDS Next — cloud-native PMS vendors active in the GCC/hospitality space; not deeply researched in this pass since Al Noor's five-star, enterprise, multi-property profile points toward the enterprise tier above. Flagged here so the eventual RFP vendor list isn't built on enterprise-tier assumptions alone without checking whether a client requirement (e.g., faster implementation, lower cost) would favor this tier instead.

## What this means for the RFP (not yet decided)

1. **Do not pre-select a vendor shortlist before discovery is complete.** The brief hasn't confirmed budget, current systems, or deployment preference (cloud vs. on-prem) — all of which materially change which tier of vendor is even eligible (see discovery questionnaire Q5.1, Q5.4).
2. **"No public pricing"** is the norm at the enterprise tier[^1] — the RFP's commercial-proposal section needs to be structured to extract comparable cost data (license/subscription model, implementation cost, per-property vs. group pricing, support cost) rather than relying on public price lists.
3. Given the UAE-specific regulatory integration requirement identified in [`regulatory-considerations.md`](regulatory-considerations.md) (government guest-reporting systems), any vendor shortlist should explicitly ask about existing UAE/GCC integration experience — this is a genuine differentiator, not a generic RFP checkbox.

*This research informs the eventual RFP vendor outreach list in `06-rfp-and-commercial/` — it does not itself constitute RFP content.*

[^1]: Roommaster, "Oracle OPERA vs Infor HMS: 2026 Comparison Guide" — see [`sources.md`](sources.md).
[^2]: Roommaster, "Shiji Alternatives: 6 Best Hotel PMS Options for Hotel Groups" — see [`sources.md`](sources.md).
