# Maturity Gap Analysis

**Date:** 2026-07-16
**Author:** Anush Sureandren - Software Testing Engineer
**Project:** Ecommerce Project
**Committed location:** https://github.com/asureandren/Build-Your-AI-Factory

---

## Scorecard

| Dimension | Level (L1 / L2 / L3) | Score (1.0 / 2.0 / 3.0) | Evidence (2–3 sentences) |
|---|---|---|---|
| AI Capabilities | L2 | 2.0 | The team uses Claude 3.5 Sonnet via EPAM DIAL for generating acceptance criteria, test cases, code reviews, and pull request descriptions on every sprint story. 5 out of 7 developers consistently use AI assistance for their daily coding and documentation tasks, with approximately 60% of sprint deliverables involving AI-generated first drafts. No autonomous agents are in use — all AI outputs require human review and editing before delivery. |
| Reusability | L2 | 2.0 | The team has a /docs/prompts/ folder in the repository with 2 committed prompt templates, including the acceptance criteria generator validated in Kata 2 by a peer reviewer. Priya Menon successfully ran the shared template independently without author assistance, confirming the template is self-explanatory. However, only 2 of 7 team members have contributed shared templates — the remaining 5 still use personal, unshared prompts stored locally or in individual DIAL histories. |
| AI Champions | L1 | 1.0 | Anush Sureandren informally helps teammates with AI tools, prompt writing, and model selection, but there is no formal AI Champion designation, management mandate, or allocated time for enablement activities. When Anush is on leave or in deep focus work, AI-related questions go unanswered and teammates revert to manual approaches or suboptimal prompts. No other team member has stepped into an enablement role, and there is no Champions network or cross-team coordination. |
| Performance Tracking | L1 | 1.0 | Team members anecdotally report that AI saves them 30–60 minutes per day, but no formal measurement exists and no one has validated these estimates. There is no dashboard, spreadsheet, or report tracking AI tool usage frequency, time saved per task, cost per query, or quality impact. Sprint retrospectives occasionally mention AI benefits qualitatively but no metrics are recorded, compared sprint-over-sprint, or reported to management. |
| DAU | L2 | 2.0 | Based on EPAM DIAL usage logs and team self-reporting during the last sprint retrospective, approximately 5 out of 7 team members (71%) use AI tools daily for coding, testing, or documentation tasks. The remaining 2 team members (a junior developer and the Scrum Master) use AI tools 2–3 times per week but not daily. This meets the >70% threshold for L2 but falls short of the >80% required for L3. |
| **Average** | | **1.6** | (2.0 + 2.0 + 1.0 + 1.0 + 2.0) ÷ 5 = 8.0 ÷ 5 = 1.6 |
| **Overall Level** | **L1** | | 1.6 falls within the 1.0–1.9 range = L1 (At Risk) |

---

## Gap Analysis

### Gap 1

**Dimension:** AI Champions
**Current level:** L1
**Why this gap is most damaging:** Without a designated champion with a formal mandate, AI adoption is fragile — it depends entirely on one person's voluntary effort, and when that person is unavailable the team loses velocity gains and reverts to manual processes, creating inconsistent delivery speed across sprints.
**Root cause:** There is no management mandate, role definition, or allocated time budget for an AI Champion function, so enablement depends entirely on individual volunteerism with no organizational backing or accountability structure.

---

### Gap 2

**Dimension:** Performance Tracking
**Current level:** L1
**Why this gap is most damaging:** Without measured productivity metrics, the team cannot demonstrate ROI to justify continued AI tool investment, cannot identify which AI practices actually deliver time savings versus which are ineffective, and cannot set improvement targets — making it impossible to move any other dimension from L2 to L3.
**Root cause:** No one has defined what specific AI productivity metrics to measure, there is no tooling or automated process to collect usage and outcome data, and no recurring review cadence exists to analyze and act on the data.

---

## 30-Day Improvement Plan

### Step 1 — addresses Gap 1

| Field | Value |
|---|---|
| **Action** | Draft a one-page AI Champion role description (responsibilities, time allocation, expected outcomes), present it to the team lead for formal approval, and announce the designated champion in the team Slack channel with a weekly 30-minute "AI Office Hour" added to the shared team calendar. |
| **Owner** | Anush Sureandren |
| **Timeline** | 2026-07-30 |
| **Success metric** | AI Champion role is formally approved by team lead (approval message received), announced in team Slack channel, and ≥4 weekly AI Office Hour sessions are scheduled on the team calendar through August 2026. |

---

### Step 2 — addresses Gap 2

| Field | Value |
|---|---|
| **Action** | Create a shared Google Sheet tracking 3 AI productivity metrics (number of AI-assisted tasks per day per person, estimated minutes saved per task, and AI output acceptance rate — percentage used without major edits), collect baseline data from all team members for 2 complete sprints, and review results in the Sprint 16 retrospective. |
| **Owner** | Anush Sureandren |
| **Timeline** | 2026-08-15 |
| **Success metric** | Spreadsheet contains ≥30 data points across ≥5 team members covering 2 complete sprints (Sprint 15 and Sprint 16), and metrics are presented with a 5-minute summary in the Sprint 16 retrospective meeting on 2026-08-15. |

---

## Peer Review

**Reviewer:** Sai krishna
**Date reviewed:** 2026-07-16

| Review question | Reviewer answer |
|---|---|
| Is the evidence for each dimension specific and observable — not aspirational? | Yes — all evidence cites specific numbers (5 of 7 developers, 71% DAU, 2 committed templates) and observable behaviours rather than future plans or intentions. |
| Which score do you challenge, and why? | I challenge AI Capabilities at L2 — while 5 of 7 developers use AI, the "60% of deliverables" claim is an estimate without measurement. Given that Performance Tracking is L1 (no metrics exist), we cannot verify the >50% threshold, and the score may be closer to L1 until data is collected. |
| Is each root cause a structural/behavioural cause — not a symptom? | Yes — both root causes identify missing organizational structures (no mandate or role definition for Champions; no defined metrics, tooling, or cadence for Tracking) rather than surface symptoms. |
| Are the success metrics measurable without asking the author? | Yes — both metrics are independently verifiable: anyone can check the team calendar for scheduled office hours and count data points in the shared spreadsheet without needing the author to confirm. |
| Would you sign off on this plan as a teammate? | Yes — the actions are realistic within 30 days, the owner is named and committed, and the metrics will give us a clear baseline; I would add that once Performance Tracking reaches L2, we should re-score AI Capabilities with actual data. |

---

## Revision History

| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | 2026-06-17 | Initial Commit | Anush Sureandren |
