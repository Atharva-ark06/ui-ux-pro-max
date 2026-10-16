---
name: design-system
description: Plan or improve a maintainable UI design system with semantic tokens, typography, spacing, component states, and usage rules.
---

# Design System Planning

## Workflow
1. Inventory repeated colors, type styles, spacing, borders, radii, shadows, and interaction patterns.
2. Define semantic roles such as `color.text.primary`, `color.surface.canvas`, and `color.action.primary`.
3. Specify foreground, surface, border, action, focus, success, warning, and danger roles.
4. Define typography by font, size, weight, line height, and intended use.
5. Choose a spacing scale and document shape/elevation rules.
6. Specify component states: default, hover, focus-visible, active, disabled, loading, invalid, and success as needed.
7. Document responsive behavior and legitimate exceptions.
8. Apply the system to representative screens and verify contrast, hierarchy, and consistency.

## Illustrative CSS tokens
```css
:root {
  --color-text-primary: #172033;
  --color-text-muted: #596579;
  --color-surface-canvas: #f7f8fb;
  --color-surface-raised: #ffffff;
  --color-border-subtle: #dce2eb;
  --color-action-primary: #2457d6;
  --space-1: 0.25rem;
  --space-2: 0.5rem;
  --space-3: 0.75rem;
  --space-4: 1rem;
  --radius-control: 0.5rem;
}
```

These values are examples, not universal defaults. Check contrast for the final foreground/background combinations.

## Deliverables
- Semantic token table with values and purpose.
- Typography scale with usage guidance.
- Component state matrix.
- Responsive rules for key layouts.
- Adoption notes and documented exceptions.

## Guidelines
- Prefer semantic tokens over unexplained magic values.
- Keep the system proportional to the product.
- Avoid encoding meaning with color alone.
- Document exceptions rather than silently duplicating tokens.
