---
name: ui-ux-audit
description: Audit an interface for usability, hierarchy, interaction clarity, accessibility, and responsive behavior.
---

# UI/UX Audit

## Purpose
Produce a prioritized, evidence-based review of an interface without recommending redesign for its own sake.

## Workflow
1. Identify the audience, primary task, platform, constraints, and success criteria.
2. Map the key journey, including loading, empty, error, disabled, and completion states.
3. Review visual hierarchy, readability, consistency, navigation, and clarity of the primary action.
4. Check interaction feedback, form labels, keyboard access, visible focus, contrast, and responsive behavior.
5. Separate directly observed problems from hypotheses that need user research or runtime testing.
6. Prioritize findings by impact and frequency.
7. Recommend the smallest useful fix and define how to verify it.

## Finding template
- **Location:** page, flow, or component.
- **Evidence:** observed behavior or supplied code.
- **User impact:** what task becomes harder or impossible.
- **Priority:** Critical / High / Medium / Low.
- **Recommendation:** concrete change.
- **Verification:** manual test or measurable outcome.

## Guidelines
- Do not claim WCAG conformance from screenshots alone.
- Avoid redesigning elements without a user problem or supporting evidence.
- Do not rely on color alone to communicate status.
- Include assumptions and testing limitations in the final summary.
