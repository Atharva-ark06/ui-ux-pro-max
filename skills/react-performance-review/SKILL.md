---
name: react-performance-review
description: Diagnose and improve React interface performance without sacrificing correctness or accessibility. Use when pages feel slow, renders are excessive, bundles grow, or interactions lag.
---

# React Performance Review

## Measure before optimizing
1. Identify the user-visible symptom and the affected route or interaction.
2. Reproduce it with representative data and a realistic device profile.
3. Use available browser performance tools, React profiling, bundle analysis, or framework diagnostics.
4. Record a baseline and choose a measurable goal.
5. Optimize the bottleneck supported by evidence rather than applying memoization everywhere.

## Investigation order
- **Network and startup:** oversized JavaScript, duplicate dependencies, render-blocking resources, image payloads, and unnecessary client-only code.
- **Rendering:** expensive calculations during render, broad context updates, unstable component boundaries, and large lists.
- **Interaction:** synchronous work on the main thread, expensive event handlers, layout thrashing, and repeated requests.
- **Data:** over-fetching, duplicate requests, missing pagination, excessive client transformations, and cache invalidation issues.
- **Assets:** incorrect image dimensions, missing responsive sources, excessive font variants, and animation-heavy effects.

## React-specific practices
- Keep state close to the components that need it.
- Avoid effect-driven state synchronization when values can be derived during render.
- Use stable keys that represent identity, not array positions for reorderable collections.
- Apply memoization only when measured work and stable inputs justify its complexity.
- Use list virtualization for genuinely large collections where it improves user experience.
- Split code by meaningful routes or features when it reduces initial work.
- Preserve semantic HTML, keyboard interaction, and focus behavior during performance refactors.

## Safe optimization loop
1. Capture a reproducible baseline.
2. Form one hypothesis.
3. Make one focused change.
4. Repeat the same measurement.
5. Run relevant tests and inspect behavior under slow network or CPU conditions.
6. Compare results and remove optimizations that add complexity without measurable value.

## Report
State the measured bottleneck, before/after data, test environment, changed files, and remaining trade-offs. If measurements are unavailable, label recommendations as hypotheses rather than proven improvements.
