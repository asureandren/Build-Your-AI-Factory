---
case: "Meridian — mid-market omnichannel retail"
date: 2025-01-15
source_kata: "02-primary-signal.md"
audit_type: "adversarial trust audit"
---

# Research Audit — Trust Ledger

**Playground:** Mid-market omnichannel grocery retail · Western Europe (EU) · €1–5B revenue

---

## Survival Count

**15 claims in → 11 survived (4 cut)**

| Verdict | Count |
|---------|-------|
| Sourced | 9 |
| Unverified (kept as hypothesis) | 2 |
| Cut | 4 |

---

## Trust Ledger

| ID | Claim (abbreviated) | Source Cited | Tag | Reason |
|----|---------------------|-------------|-----|--------|
| C1 | Quick-commerce exits (Getir/Gorillas) pushed demand to omnichannel players | IGD, Mar 2024 | **Sourced** | Widely reported event; IGD coverage confirmed directionally |
| C2 | Click-and-collect volumes rose 12–18% for mid-market grocers | IGD, Mar 2024 | **Cut** | Specific percentage range unverifiable; flagged as classic AI confabulation pattern (plausible range, paywalled source). No second source found. |
| C3 | Private-label share reached 38% (up from 34% in 2022) | IGD, Mar 2024 | **Unverified** | PLMA reports ~36.2% for 2023. Direction correct (PL share growing); specific numbers likely overstated. Kept as directional hypothesis only. |
| C4 | Last-mile cost rose to €8.20/order (from €6.70 in 2022) | IGD, Mar 2024 | **Unverified** | No publicly available source confirms this exact figure. Multiple consultancies cite different ranges (€7–12). Direction correct; number uncheckable. **Weakest kept claim — see below.** |
| C5 | Carrefour Sprint launched across 12 French cities via Uber Eats Q2 2024 | Reuters (Ahold article), Jan 2024 | **Cut** | Misattribution. The cited Reuters article covers Ahold Delhaize, not Carrefour. Carrefour Sprint was announced via Carrefour's own press release. Source does not say this. |
| C6 | Ahold Delhaize committed €600M to automated MFCs, 40% cost reduction target by 2026 | Reuters, Jan 2024 | **Sourced** | Reuters article confirmed; aligns with Ahold Delhaize Capital Markets Day disclosures |
| C7 | Lidl expanded Lidl Plus to 31 EU markets by mid-2024 | Reuters (Ahold article), Jan 2024 | **Cut** | Misattribution. Same Reuters article about Ahold Delhaize does not cover Lidl Plus. Lidl Plus expansion reported by Lidl press office and trade press, not this source. |
| C8 | EU DSA full enforcement from 17 February 2024 | European Commission, Feb 2024 | **Sourced** | Confirmed on official EC DSA page |
| C9 | Irish DPC issued €1.2B cumulative GDPR fines in 2023 | European Commission, Feb 2024 | **Cut** | Conflation: €1.2B was a single fine against Meta (Sep 2023), not "cumulative retail fines." Source misattributed to EC (should be Irish DPC). The claim as written is materially misleading. |
| C10 | EU CSRD effective Jan 2024 for companies >€40M revenue; Scope 3 disclosure | European Commission, Feb 2024 | **Sourced** | Confirmed on official EC CSRD page. Threshold slightly simplified but correct for this segment. |
| C11 | Colruyt CEO: online cost-to-serve "3 to 4 percentage points above in-store margin" | Colruyt FY2024 earnings call, Jun 2024 | **Sourced** | Public earnings call transcript; specific executive quote with verifiable source |
| C12 | Colruyt CEO: omnichannel loyalty members spend 2.4x more than single-channel | Colruyt FY2024 earnings call, Jun 2024 | **Sourced** | Same verifiable transcript source |
| C13 | Jumbo app user abandoned order due to delivery fee jump (€2.99→€7.95 under €80) | Google Play review, Sep 2024 | **Sourced** | Public platform review with date and username; acceptable verbatim provenance |
| C14 | Delhaize loyalty user forced to re-consent or lose points | Trustpilot review, Mar 2024 | **Sourced** | Public platform review with date and username; acceptable verbatim provenance |
| C15 | Carrefour teardown: no visible DSA transparency labels found | First-party observation, Jan 2025 | **Sourced** | Primary research by auditor; point-in-time observation documented |

---

## Cuts — One-Line Reasons

| ID | Cut Reason |
|----|-----------|
| C2 | Specific 12–18% figure unverifiable; classic AI confabulation pattern; no second source |
| C5 | Misattribution — cited Reuters article is about Ahold Delhaize, not Carrefour Sprint |
| C7 | Misattribution — same Reuters article does not cover Lidl Plus expansion |
| C9 | Conflation of single €1.2B Meta fine with "cumulative retail fines"; source misattributed to EC instead of Irish DPC |

---

## Propagation of Cuts

The following downstream impacts must be addressed in later katas:

| Cut | Impact on Pain Points | Action |
|-----|----------------------|--------|
| C2 cut | Pain Point 1 (fulfilment economics) loses the "12–18% click-and-collect uplift" supporting data | Remove from any ROI calculation; rely on C11 (Colruyt 3–4 pp gap) and C13 (user abandonment) instead |
| C5 cut | Pain Point 2 (margin levers neutralised) loses Carrefour Sprint as a sourced competitive threat | Re-source from Carrefour's own press release if needed; or note as "reported but unverified source" |
| C7 cut | Pain Point 2 loses Lidl Plus "31 markets" as a sourced claim | Re-source from Lidl press office or trade press (The Grocer) if needed |
| C9 cut | Pain Point 3 (regulatory shock) loses the "€1.2B cumulative" enforcement figure | Replace with: "Record €1.2B single fine against Meta by Irish DPC (Sep 2023) signals escalating enforcement" — correctly attributed |

---

## Triangulation Risk Flag

**Single-source cluster:** Claims C1, C3, and C4 all depend on one source (IGD Retail Analysis, March 2024). If IGD's report does not exist in the exact form cited, or uses different methodology, all three claims weaken simultaneously.

- C1 survives because the underlying event (q-commerce exits) is independently reported.
- C3 and C4 are tagged **unverified** and should not be used as precise figures in ROI calculations without a second source.

---

## Weakest Kept Claim

**C4: "Average last-mile delivery cost per order rose to €8.20 in 2024 (from €6.70 in 2022)"**

**Why it's the weakest:**
- No publicly verifiable source confirms this exact figure
- Multiple consultancies cite different ranges (Capgemini: €10+; McKinsey: €7–12; Bain: varies by density)
- A single pan-European average obscures massive country-by-country variation
- The figure is suspiciously precise for a continent-wide average

**Why I'm keeping it:**
- The *direction* (last-mile costs rising significantly) is confirmed by multiple sources
- Verbatim 1 (C13) provides qualitative confirmation that delivery costs are customer-visible and drive abandonment
- Colruyt's 3–4 pp margin gap (C11) is consistent with rising fulfilment costs
- The figure is useful as an order-of-magnitude anchor, even if imprecise

**CONFIRM BEFORE EXEC REVIEW:** Replace €8.20 with a sourced figure from a named consultancy report (e.g., Capgemini "Last Mile Delivery Challenge" or McKinsey "Grocery's Next S-Curve") before this number appears in any executive-facing material.

---

## Adversarial Method Used

1. Manual source verification (open cited sources, check existence and content)
2. Triangulation check (single-source-wearing-three-hats)
3. AI adversarial prompt: *"Which of these claims would a skeptic call AI-generated filler, and why?"*
4. Reconciliation of AI critique against manual tags

---

## Final Verdict Summary

| Category | Claims |
|----------|--------|
| **Safe to build on** (sourced) | C1, C6, C8, C10, C11, C12, C13, C14, C15 |
| **Use directionally only** (unverified) | C3, C4 |
| **Do not use** (cut) | C2, C5, C7, C9 |

---

*Audit completed in support of Kata 1.W series · Meridian Reference Case*
*Auditor: Anush Sureandren · Date: 24 July 2026*