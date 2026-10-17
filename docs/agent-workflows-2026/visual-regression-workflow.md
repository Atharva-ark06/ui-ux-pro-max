# Visual Regression Testing Workflow

Visual regression tests compare rendered UI with an approved baseline.

## Build a stable baseline

- Pin browser and viewport sizes.
- Control fonts, animation, network data, and fixtures.
- Capture key component states, not only the homepage.
- Use deterministic test data rather than live production content.

## Review each diff

1. Run the screenshot tests.
2. Inspect each difference.
3. Separate intentional design changes from regressions.
4. Update a baseline only after reviewing the reason.
5. Fix flaky inputs instead of repeatedly approving snapshots.

## Suggested coverage

- Desktop and narrow/mobile viewports
- Navigation open and closed
- Form validation errors
- Empty or loading states
- Theme variants where supported

Screenshot comparisons do not prove accessibility or behavior. Pair them with functional tests and keyboard checks.

Reference: https://playwright.dev/docs/test-snapshots
