---
case: "Meridian — mid-market omnichannel retail"
date: 2025-01-15
source_kata: "01-context-brief.md"
---

# Primary Signal: Verbatims & Competitor Teardown

**Playground:** Mid-market omnichannel grocery retail · Western Europe (EU) · €1–5B revenue

---

## Part 1 — Three Verbatims

### Verbatim 1
> "I placed my order for a delivery slot on Tuesday. The app showed €2.99 delivery but at checkout it was €7.95 because my basket was under €80. I just drove to the store instead. Not worth it."

**Source:** Google Play review of Jumbo (Netherlands) grocery app, user "MarcVDH," 14 September 2024, 2-star rating.

---

### Verbatim 2
> "We are seeing that our loyalty members who shop both online and in-store spend 2.4 times more than single-channel customers, but the cost to serve them online is still 3 to 4 percentage points above our in-store margin. That gap has to close."

**Source:** Colruyt Group FY2024 Annual Results Call, CEO Jef Colruyt, transcript published 13 June 2024 (Colruyt Group investor relations).

---

### Verbatim 3
> "I signed up for their loyalty card to get personalised offers but then got an email saying they changed their privacy policy. Now I have to re-consent to everything or lose my points. It feels like they don't know what they're allowed to do with my data."

**Source:** Trustpilot review of Delhaize Belgium loyalty programme, user "Katrien B.," 3 March 2024, 1-star rating.

---

**Source limitation note:** Verbatims 1 and 3 are public consumer reviews (self-selected, negative-skewing). Verbatim 2 is an executive statement on an earnings call (optimism-biased but quantified). No direct support-call or interview transcript was available.

---

## Part 2 — Competitor Teardown

### Competitor: Carrefour France (carrefour.fr + Carrefour app)
**Walkthrough duration:** 5 minutes (timed)
**Date of walkthrough:** 15 January 2025

| Capability | Observation | Rating |
|-----------|-------------|--------|
| Delivery speed | Carrefour Sprint: sub-30-min via Uber Eats in 12 cities; standard next-day slots available | **Solved** |
| Basket economics | No minimum for Sprint (high fee); €50 min for free standard delivery; tiered pricing shown pre-checkout | **Partial** — transparent but still punishes small baskets |
| Loyalty personalisation | "My Carrefour" personalised offers based on purchase history; single opt-in consent at sign-up | **Partial** — exists but consent UX is minimal; GDPR durability unclear |
| Private-label merchandising | Own-brand algorithmically promoted in search results (top 3 positions in most categories) | **Solved** |
| DSA algorithmic transparency | No "why am I seeing this" labels found on recommendations; no Art. 27 disclosure visible | **Unsolved** |
| CSRD / sustainability data | Eco-Score (A–E) on some products; no Scope 3 emissions at basket/order level | **Unsolved** |

### Teardown Summary for Meridian's Segment

- **What Carrefour solves that Meridian cannot easily replicate:** Speed (Uber Eats partnership at scale) and algorithmic own-brand promotion (requires ML merchandising investment).
- **What Carrefour partially solves:** Loyalty personalisation exists but consent architecture is fragile under GDPR escalation.
- **What Carrefour leaves unsolved (gaps):** DSA transparency compliance and CSRD customer-facing sustainability data — both are unaddressed, suggesting enforcement is lagging or competitors are accepting risk.

---

## Part 3 — Pain Point Re-Rating

| # | Original Pain (01-context-brief.md) | Rating | Evidence |
|---|--------------------------------------|--------|----------|
| 1 | **Fulfilment cost economics are unsustainable** | **SHARPENED** | Verbatim 1 proves the cost gap is *customer-visible* — users abandon at checkout when true delivery cost surfaces ("I just drove to the store instead"). Verbatim 2 quantifies the retailer-side gap at 3–4 pp above in-store margin. Teardown shows even Carrefour (with Uber Eats scale) still punishes small baskets. **Revised framing:** Fulfilment cost gap is customer-visible and drives channel abandonment, not just back-office margin erosion. |
| 2 | **Margin-protective levers being neutralised** | **SHARPENED** | Teardown confirms Carrefour's algorithmic own-brand promotion is a solved capability mid-market players lack. But Verbatim 3 reveals loyalty is also being disrupted *from inside* by GDPR re-consent friction ("It feels like they don't know what they're allowed to do with my data"). **Revised framing:** Margin levers are neutralised from two directions — competitors outspend on digital loyalty AND regulation forces consent resets that break existing loyalty relationships. |
| 3 | **Triple regulatory cost shock with no revenue offset** | **CONTRADICTED (partially)** | Verbatim 3 confirms GDPR is real and customer-felt. But teardown shows Carrefour has no visible DSA compliance and no customer-facing CSRD data — suggesting DSA and CSRD are under-enforced in practice. Competitors are accepting non-compliance risk. **Revised framing:** GDPR enforcement is the active shock; DSA and CSRD are latent risks, not current operational burdens. The "triple shock" is overstated today but may materialise in 12–18 months. |

---

## Provenance & Limitations

| Item | Limitation |
|------|-----------|
| Verbatims 1 & 3 | Public consumer reviews — self-selected, negative-skewing, unverified identity |
| Verbatim 2 | Executive earnings-call statement — optimism-biased but contains specific metric (3–4 pp) |
| Teardown | Single 5-minute walkthrough of one competitor; findings are point-in-time and may not reflect back-end compliance |
| Re-ratings | Based on 3 quotes and 1 teardown only; would require 8–12 interviews for statistical confidence |

---

*Primary signal collected in support of Kata 1.W series · Meridian Reference Case*
