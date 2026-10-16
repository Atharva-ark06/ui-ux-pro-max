---
name: automated-test-strategy
description: Design a practical automated testing strategy across unit, integration, end-to-end, and regression tests. Use when adding a feature, fixing a bug, reviewing test gaps, or choosing what to automate first.
---

# Automated Test Strategy

## 1. Understand the risk
Before writing tests, identify the user-visible behavior, important invariants, failure modes, data boundaries, and the cost of a regression. Prioritize high-impact flows over arbitrary coverage targets.

## 2. Choose the test layer
- **Unit:** pure logic, formatting, calculations, validation rules, and isolated edge cases.
- **Integration:** database access, API boundaries, queues, filesystem behavior, and collaboration between modules.
- **End-to-end:** a small number of critical user journeys across the real application boundary.
- **Contract:** request/response schemas and compatibility between independently deployed services.
- **Visual regression:** stable layouts and component states where visual differences matter.
Use the narrowest layer that gives trustworthy evidence. Do not use a slow browser test for every small conditional.

## 3. Build meaningful cases
For each behavior, include:
- Typical valid input.
- Boundary values and empty input.
- Invalid or malformed input.
- Permission or authentication failures where relevant.
- Network, dependency, or persistence failures.
- Regression case for the reported defect.
- Recovery or retry behavior when the user can recover.

## 4. Keep tests reliable
- Control time, randomness, and external dependencies when practical.
- Use unique test data and clean up resources.
- Avoid relying on test order or shared mutable state.
- Prefer observable outcomes over implementation details.
- Use explicit waits for a meaningful condition, not arbitrary sleeps.
- Do not silence flaky tests without tracking the underlying cause.

## 5. Work in the existing project
1. Inspect the current test framework and naming conventions.
2. Reproduce the failure before changing code when possible.
3. Add the smallest test that fails for the bug or missing behavior.
4. Implement the fix, then run the focused test.
5. Run related tests and the repository's documented checks.
6. Report exact commands and results; distinguish skipped tests from passing tests.

## 6. Coverage and quality
Coverage can reveal untested code but cannot prove that assertions are useful. Review whether tests would fail if the behavior were broken. Avoid testing private implementation details unless they are themselves a contract.

## Completion report
Summarize the behavior covered, tests added, commands executed, failures or skips, and any remaining risk. Never claim a suite passed if it was not run.
