---
name: accessibility-review
description: Review web interfaces for semantic HTML, keyboard access, focus, forms, contrast, motion, and assistive-technology barriers.
---

# Accessibility Review

## Review workflow
1. Check semantic landmarks, heading order, native controls, and meaningful link/button names.
2. Navigate with Tab and Shift+Tab; verify controls work with expected keyboard keys and there are no traps.
3. Confirm focus is visible and not obscured by sticky headers, dialogs, or overlays.
4. Check persistent form labels, instructions, required formats, and field-specific validation messages.
5. Verify important status changes are announced or otherwise perceivable without relying on color alone.
6. Measure text contrast and inspect non-text indicators that communicate meaning.
7. Review informative image alternatives, decorative image handling, and captions where needed.
8. Test zoom, narrow viewport reflow, long content, and touch operation.
9. Check that motion-sensitive effects respect reduced-motion preferences.
10. Retest fixes with automated checks and manual keyboard/screen-reader testing.

## Report each finding
- Page/component and reproduction steps.
- Expected versus actual behavior.
- User impact and severity.
- Applicable WCAG criterion, when verified.
- Recommended fix and retest steps.

## Cautions
- Automated tools detect only a subset of accessibility issues.
- A screenshot alone cannot establish WCAG conformance.
- Do not describe a product as fully accessible after a limited review.
- Prefer native HTML semantics; add ARIA only when native semantics are insufficient.
- Avoid positive tabindex values and preserve a logical focus order.
