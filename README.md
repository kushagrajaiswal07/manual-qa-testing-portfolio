# Manual QA Testing Portfolio — E-commerce Web Application

An independent manual QA portfolio project demonstrating test design, black-box testing, exploratory testing, and structured defect documentation for an e-commerce storefront.

> **Portfolio note:** This repository is a sanitized presentation of testing practice. It is not an endorsement by, or a claim of employment with, any company. Publish only if the original assessment terms permit reuse of your work. If they do not, use this structure with a separate public demo application and original test data.

## Project overview

The goal was to evaluate customer-facing e-commerce flows through the visible user interface, without source-code or backend access.

### Coverage

- Homepage and navigation
- Product browsing, search, filters, and sorting
- Cart and wishlist behavior
- Registration and login checks
- Checkout fields and validation
- Order summary and displayed totals
- UI behavior, loading states, and browser navigation

## Deliverables

- [`test-cases.xlsx`](test-cases.xlsx) — 57 test cases with steps, expected and actual results, execution status, and notes.
- [`bug-reports.xlsx`](bug-reports.xlsx) — 10 recorded findings with reproduction steps, expected versus actual behavior, impact, and verification notes.
- [`test-summary.md`](test-summary.md) — scope, key observations, limitations, and areas requiring follow-up.

## Testing approach

1. Identify core user journeys and relevant edge cases.
2. Write reproducible test steps and expected outcomes.
3. Execute tests through the visible interface.
4. Compare observed behavior with expected behavior.
5. Record findings with clear reproduction steps and impact.
6. Mark ambiguous observations as provisional or requiring verification rather than presenting them as confirmed defects.

## Skills demonstrated

Manual testing · Test case design · Exploratory testing · Black-box testing · Positive and negative testing · Boundary and input validation · Defect reporting · Severity assessment · Test documentation

## Important interpretation

The bug report intentionally distinguishes observed behavior from confirmed product defects. Some findings require clarification of intended business rules or additional evidence before they can be classified as defects. No actual payment was completed as part of the recorded checks.

## Suggested interview discussion

- How I converted user workflows into test scenarios and cases
- How I made bug reports reproducible
- How I handled ambiguous expected behavior
- How I prioritized issues affecting checkout, pricing, and customer experience
- What additional evidence or regression checks I would gather before closing a defect
