# Color Contrast Review Workflow

Contrast checks help ensure text and meaningful interface elements remain perceivable.

## Process
1. Identify text, icons, borders, focus indicators, and states that convey information.
2. Use the actual foreground and background colors, including overlays and opacity.
3. Check contrast with an appropriate tool.
4. Test default, hover, focus, disabled, and error states.
5. Verify themes and gradients, not only the base token.
6. Record exceptions and manually inspect real rendered content.

## Avoid
- Using color alone to signal errors or status.
- Assuming a token name guarantees sufficient contrast.
- Testing only the design canvas when runtime overlays change colors.
- Treating an automated scan as complete accessibility certification.

Reference: https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html