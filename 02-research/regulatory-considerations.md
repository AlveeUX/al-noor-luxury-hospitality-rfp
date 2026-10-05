# UAE/GCC Regulatory Considerations for a Hotel Management System

**Purpose:** Discovery question 5.3 asked whether UAE-specific regulatory requirements apply. Rather than guess, this is real research into what actually exists — so the eventual requirements set is grounded in confirmed regulation, not assumption.

## 1. Government guest-registration reporting

UAE hotels are required to report guest data to local tourism/economic authorities. In Dubai specifically, guest data (full name, identification number, nationality, arrival and departure dates) must be submitted to the Department of Economy and Tourism (DET, formerly DTCM) via a system referred to as "DTCM HH 2.0," and in some cases also to EMAAR.[^1] Commercial compliance vendors offer PMS-integrated automation for this submission so that verified guest data flows from the PMS without manual double-entry or portal uploads.[^1]

**Implication for Al Noor:** this is very likely a **mandatory, non-negotiable integration requirement**, not an optional nice-to-have — and because Al Noor's five properties sit in different emirates, the specific reporting authority and system may differ *by emirate* (Dubai's DET/DTCM system is confirmed; other emirates may have their own tourism-authority systems not yet researched). This should be a direct discovery follow-up question per property, and a mandatory line item in the RFP's integration requirements.

**Confidence:** Medium — confirmed for Dubai from a vendor source describing the integration; not independently verified against a primary government source in this research pass, and not yet confirmed for the other emirates where Al Noor's hotels may be located. Should be validated against official Dubai DET / UAE government sources before being finalized as a hard requirement in the RFP.

## 2. Data protection — Federal Decree-Law No. 45 of 2021 (UAE PDPL)

The UAE's federal data protection law applies to private-sector organizations processing personal data within the UAE (plus foreign companies processing UAE residents' data), with notable carve-outs for entities registered in the DIFC and ADGM financial free zones, which have their own data protection regimes.[^2] Key obligations include obtaining explicit, informed consent, limiting processing to a specific lawful purpose, implementing security safeguards, honoring data-subject access/correction/erasure rights, appointing a Data Protection Officer where required, and meeting adequacy or contractual safeguards for cross-border data transfers.[^2] Enforcement sits with the UAE Data Office, with penalties reported up to AED 5 million (~USD 1.36 million).[^2]

**Implication for Al Noor:** a hotel system handling guest PII (passport/ID numbers, payment data, contact details) across five properties is squarely in scope of this law. This affects:
- **Vendor data-handling requirements** in the RFP's security section (consent capture, data subject access/erasure support, breach notification capability)
- **Cross-border hosting questions** — if a vendor's cloud infrastructure sits outside the UAE, cross-border transfer safeguards need explicit confirmation (ties to discovery Q5.4, cloud vs. on-prem)
- **DPO assignment** — worth confirming in discovery whether Al Noor already has a Data Protection Officer or whether this project triggers that requirement

**Confidence:** Medium-high — sourced from a compliance-platform summary of the law rather than the primary legislative text; the general obligations are consistent with how PDPL is commonly described, but a real engagement would cite the Official Gazette text directly rather than a secondary summary.

## 3. Not yet researched / flagged for follow-up

- VAT e-invoicing requirements for billing/folio modules
- Emirate-specific tourism dirham / municipality fee calculation (varies by emirate — relevant to the billing module)
- PCI-DSS requirements for payment card handling (industry-standard, not UAE-specific, but should be in the security section regardless)
- Free-zone-specific rules if any Al Noor property sits within a free zone (e.g., DIFC) rather than mainland UAE

*These gaps are intentionally left open rather than filled with assumptions — see [`sources.md`](sources.md) for research-confidence notes and [`../DECISIONS.md`](../DECISIONS.md) for how open items convert into RFP questions for vendors or follow-up discovery questions for the client.*

[^1]: ChargeAutomation, "Guest Compliance — UAE (Dubai) – (DTCM & EMAAR)" — see [`sources.md`](sources.md).
[^2]: Clym, summary of UAE Federal Decree-Law No. 45 of 2021 — see [`sources.md`](sources.md).
