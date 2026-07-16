# Prompt Template: [Task Name]

**Date:** 2026-07-16
**Author:** Anush Sureandren - Software Testing Engineer
**Project:** Ecommerce Project
**Model:** Claude 3.5 Sonnet via EPAM DIAL
**DIAL location:** [DIAL shared link or folder path]
**Committed location:** https://github.com/asureandren/Build-Your-AI-Factory/blob/master/prompt-template-pr-summary.md

---

## Purpose

This prompt generates acceptance criteria in Gherkin format from a product manager's user story description, for QA engineers and developers to use during sprint planning and backlog refinement.

---

## Variable Placeholders

| Placeholder | Description | Example value |
|---|---|---|
| `{{user_story}}` | The full text of the user story including role, goal, and benefit (As a... I want... So that...) | "As a registered user, I want to reset my password via email so that I can regain access to my account if I forget my password." |
| `{{number_of_edge_cases}}` | How many edge case scenarios to generate beyond the happy path | "3" |
| `{{output_language}}` | The language in which the acceptance criteria should be written | "English" |
| `{{additional_context}}` | Any extra business rules, constraints, or technical notes relevant to the story | "Password reset links must expire after 24 hours. The system must not reveal whether an email exists in the database." |

---

## Output Format Instruction

Return a numbered list of acceptance criteria in strict Gherkin format. Each criterion must have exactly one Given clause, one When clause, and one Then clause — each on its own line, indented under the scenario number. Start with the happy path as item #1, followed by edge cases. No preamble, no explanations, no commentary, no bold text, no bullet points. Maximum scenarios = 1 + {{number_of_edge_cases}}.

---

## Prompt Body

You are a senior QA engineer writing acceptance criteria for a cross-functional development team.

**Task:** Generate acceptance criteria in Gherkin (Given/When/Then) format for the following user story.

**User Story:**
{{user_story}}

**Additional Context / Business Rules:**
{{additional_context}}

**Requirements:**
- Start with the happy path scenario as item #1
- Then generate exactly {{number_of_edge_cases}} edge case scenarios
- Each scenario must have exactly one Given, one When, and one Then clause
- Each clause must be on its own line, indented under the scenario number
- Write all criteria in {{output_language}}
- Do not include explanations, preambles, headers, bold text, bullet points, or commentary
- Do not contradict the original user story or the additional context provided
- Number each scenario sequentially (1, 2, 3...)

**Output format:** Numbered list in strict Gherkin syntax only. No other text before or after the list.

---

## Test Run (Author)

**Input values used:**
- `{{user_story}}` = "As a registered user, I want to reset my password via email so that I can regain access to my account if I forget my password."
- `{{number_of_edge_cases}}` = "3"
- `{{output_language}}` = "English"
- `{{additional_context}}` = "Password reset links must expire after 24 hours. The system must not reveal whether an email exists in the database. Users cannot reuse their last 3 passwords."

**Output quality:** Output was usable as-is — all 4 scenarios used correct and consistent Gherkin syntax, covered the happy path plus three distinct edge cases, and respected all business rules from the additional context with no manual editing required before pasting into Jira.

---

## Revision History

| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | 2026-07-16 | Initial commit | Anush |
