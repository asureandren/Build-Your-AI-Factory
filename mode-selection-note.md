# Model Selection Note

**Date:** 2026-07-15
**Author:** [Anush Sureandren — Software Testing Engineer]
**Project:** [Ecommerce Project]
**Task:** [Generating Acceptance criteria for the given Userstory]
**Committed location:** (https://github.com/asureandren/Build-Your-AI-Factory)

---

## Evaluation Criteria

| # | Criterion | Why it matters for this task |
|---|-----------|------------------------------|
| 1 | Format Compliance | Must output Gherkin syntax to paste directly into Jira |
| 2 | Completeness | Must cover happy path + at least 2 edge cases |
| 3 | Accuracy | Must not contradict the original user story |

---

## Prompt Used

You are a QA analyst. Given the following user story, generate acceptance criteria in Given/When/Then (Gherkin) format. Include the happy path and at least 2 edge cases. The User story is about the login feature of the Ecommerce website.

---

## Output Comparison

### Model A: [GPT 5.0]
> Feature: User Login
  As a registered customer
  I want to log in to the ecommerce website
  So that I can access my account, view orders, and complete purchases

  Scenario: Successful login with valid credentials
    Given the user is on the login page
    And the user has a registered account
    When the user enters a valid email address
    And the user enters the correct password
    And the user clicks the "Login" button
    Then the user should be successfully logged in
    And the user should be redirected to their account dashboard or previous page
    And the user's name or account icon should be displayed in the header

### Model B: [Claude Haiku 4.5]
> Scenario: User successfully logs in with valid email and password
  Given the user is on the login page of the ecommerce website
  And the user is not already logged in
  When the user enters a valid email address "user@example.com"
  And the user enters a valid password "SecurePassword123"
  And the user clicks the "Login" button
  Then the system validates the credentials against the database
  And the user is successfully authenticated
  And the user is redirected to the dashboard/homepage
  And the user session is created with a valid authentication token
  And a welcome message "Welcome back, [User Name]" is displayed
  
  Scenario: User attempts to log in with incorrect password
  Given the user is on the login page of the ecommerce website
  And a user account exists with email "user@example.com"
  When the user enters the correct email "user@example.com"
  And the user enters an incorrect password "WrongPassword123"
  And the user clicks the "Login" button
  Then the system validates the credentials and finds a mismatch
  And the login attempt fails

---

## Scorecard

| Criterion | Model A score (1–3) | Model A evidence | Model B score (1–3) | Model B evidence |
|-----------|---------------------|------------------|---------------------|------------------|
| Format Compliance | 3 | model A |  1 | model B |
| Completeness | 2 | model A | 1 | model B |
| Accuracy | 2 | Model A | 3 | Model B |
| **Total** | 7 | | 5 | |

---

## Decision

**Selected model:** GPT 5.0

**Rationale:** I selected GPT 5.0 Model because it scored 3 in format compliance, producing gherkin syntax i can past directly into Jira. Claude's main shortcoming was inconsistent formatting.  

---

## Active Constraint

**What could change this decision within 30 days:**
If EPAM DIAL access is restricted to Claude only due to licensing, this decision would need revisiting.

---

## Revision history

| Version | Date | Change |
|---------|------|--------|
| 1.0 | 2026-07-15 | Initial commit |