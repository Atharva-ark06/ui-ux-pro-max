# Responsive Layout Review

Review layouts at content-driven breakpoints, not only at a few popular device widths.

## Review steps
1. Identify the narrowest supported viewport and the widest target viewport.
2. Check navigation, grids, forms, tables, dialogs, and long text.
3. Verify that content reflows without horizontal scrolling unless scrolling is intentional.
4. Check touch target spacing and fixed-position elements.
5. Test zoom/reflow and long localized strings where relevant.
6. Record screenshots and reproducible issues.

## Common failure modes
- Fixed widths that overflow small screens
- Text clipped by fixed-height containers
- Hover-only actions unavailable on touch or keyboard
- Dialogs extending beyond the viewport
- Controls too close together
- Breakpoints chosen for device labels instead of content needs

A responsive review should include functional and accessibility checks, not just visual snapshots.