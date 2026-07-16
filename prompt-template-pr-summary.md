# Prompt Template: [Task Name]

**Date:** YYYY-MM-DD
**Author:** [Name — Role]
**Project:** [Project name — omit client-confidential details per project policy]
**Model:** [Model used — e.g., Claude via DIAL, GitHub Copilot Chat]
**DIAL location:** [DIAL shared link or folder path]
**Committed location:** [Repo path]

---

## Purpose

[One sentence: what this prompt does, for whom, and at which SDLC stage it is used.]

---

## Variable Placeholders

| Placeholder | Description | Example value |
|---|---|---|
| `{{placeholder_1}}` | [What this variable contains] | [Realistic example] |
| `{{placeholder_2}}` | [What this variable contains] | [Realistic example] |
| `{{placeholder_3}}` | [What this variable contains] | [Realistic example] |

---

## Output Format Instruction

[Tell the model exactly what format to return. Be specific: e.g., "Return a markdown table with columns X, Y, Z. Maximum 10 rows. No preamble."]

---

## Prompt Body

[Full prompt text. Use {{placeholder}} syntax for all variable inputs. The prompt must be runnable by a teammate with zero explanation from you.]

---

## Test Run (Author)

**Input values used:**
- `{{placeholder_1}}` = [value you used]
- `{{placeholder_2}}` = [value you used]

**Output quality:** [One sentence — was the output usable as-is, or did you revise?]

---

## Peer Review

**Reviewer:** [Name — Role]
**Date reviewed:** YYYY-MM-DD
**Model used by reviewer:** [Model name]

**Reviewer input values used:**
- `{{placeholder_1}}` = [value reviewer used]
- `{{placeholder_2}}` = [value reviewer used]

| Review question | Reviewer answer |
|---|---|
| Could you run the template without asking the author anything? | Yes / No — [one sentence] |
| Was the output format what you expected? | Yes / No — [one sentence] |
| Would you use this template on your own work? | Yes / No — [one sentence] |
| One concrete improvement suggestion | [One sentence] |

---

## Revision History

| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | YYYY-MM-DD | Initial commit | [Name] |
| 1.1 | YYYY-MM-DD | Post-review update | [Name] |