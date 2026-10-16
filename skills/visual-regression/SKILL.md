---
name: visual-regression
description: Detect unintended visual changes by comparing stable, representative UI screenshots across revisions.
---
# Visual Regression Testing
1. Choose critical pages, states, viewport sizes, and representative content.
2. Stabilize fonts, animation, network data, timestamps, and other sources of screenshot noise.
3. Capture a known baseline from an approved revision.
4. Compare screenshots with a tolerance appropriate to the rendering environment.
5. Review diffs rather than blindly accepting updated baselines.
6. Separate intentional design changes from layout, overflow, typography, and asset regressions.
7. Include loading, empty, error, and interaction states where important.
8. Record browser/OS assumptions and keep baseline updates reviewable.
Visual diffs reveal appearance changes, not whether the interface remains usable or accessible.
