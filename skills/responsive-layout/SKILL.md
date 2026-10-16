---
name: responsive-layout
description: Design and implement layouts that adapt to available space without losing content, usability, or visual hierarchy.
---

# Responsive Layout

## Workflow
1. Identify the primary task and content that must remain available at every width.
2. Establish content hierarchy before choosing breakpoints.
3. Use Flexbox for one-dimensional alignment, Grid for two-dimensional structure, and normal document flow for reading content.
4. Add breakpoints where content or controls stop working well, not just at device-brand dimensions.
5. Define behavior for navigation, sidebars, tables, cards, dialogs, forms, and media at constrained widths.
6. Test long labels, missing content, validation messages, and localized strings.
7. Recheck keyboard order and focus after responsive rearrangement.
8. Test widths just above and below each breakpoint.
9. Check horizontal overflow and layout shifts.

## Example
```css
.page-grid {
  display: grid;
  grid-template-columns: minmax(0, 1fr);
  gap: 1rem;
}

@media (min-width: 48rem) {
  .page-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.5rem;
  }
}

@media (min-width: 72rem) {
  .page-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 2rem;
  }
}
```

## Validation checklist
- No unintended horizontal page scrolling.
- Content order remains logical.
- Controls remain reachable and operable.
- Important text does not overlap or truncate.
- Images preserve a suitable aspect ratio and crop.
- Sticky UI does not obscure focused controls.
- Dialogs and menus remain usable at short viewport heights.

## Guidelines
- Use fluid sizing when it improves continuity.
- Consider `minmax(0, 1fr)` for grid children containing long content.
- Avoid fixed heights for content that wraps or expands.
- Do not hide essential content simply to simplify mobile layouts.
