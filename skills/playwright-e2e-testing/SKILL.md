---
name: playwright-e2e-testing
description: Create reliable browser end-to-end tests with Playwright for critical user journeys, forms, navigation, and regression cases. Use when automating browser behavior or debugging flaky UI tests.
---

# Playwright End-to-End Testing

## Start with the user journey
1. Inspect the existing Playwright configuration, scripts, fixtures, and conventions.
2. Choose a critical user journey and define observable acceptance criteria.
3. Reuse existing fixtures and authenticated state only when the test environment permits it.
4. Prefer accessible locators such as role, label, and text; use test IDs when they express a stable testing contract.
5. Avoid selectors tied to CSS structure, generated class names, or fragile DOM positions.

## Test design
- Keep each test focused on a meaningful behavior.
- Assert visible outcomes and state transitions, not just that a click completed.
- Cover validation, empty results, network failure, and recovery where relevant.
- Use isolated test data and reset state between tests.
- Mock external systems only when the test's purpose is not to verify the real integration.
- Do not hard-code production credentials or reuse personal accounts.

## Reliability
- Use Playwright's auto-waiting and web-first assertions.
- Wait for the expected UI state or response instead of fixed sleeps.
- Avoid order-dependent tests and shared mutable data.
- Use deterministic seeds or controlled clocks where supported.
- Capture traces, screenshots, or video for failures when configured.
- If a test is flaky, investigate timing, test isolation, selectors, and dependency instability before adding retries.

## Accessibility and responsive checks
Exercise keyboard navigation and meaningful accessible names for important flows. Add viewport coverage where layout behavior is part of the acceptance criteria. Automated checks are useful signals but do not replace manual assistive-technology testing.

## Execution
Run the narrow test first, then the related suite. Confirm the configured base URL and environment before running tests that can touch external systems. Do not run destructive tests against production.

## Completion report
List test files, scenarios covered, commands run, and actual pass/fail/skip counts. Include traces or screenshots only when available, and never claim a test passed if it did not execute.
