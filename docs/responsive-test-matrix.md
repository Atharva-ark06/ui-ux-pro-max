# Responsive Layout Test Matrix

Test content behavior at representative widths rather than assuming that named device presets cover every layout failure.

| Scenario | What to inspect | Pass condition |
|---|---|---|
| Narrow phone | Navigation, forms, buttons | Core actions remain visible and operable |
| Wide phone / small tablet | Grid transitions, cards | No awkward gaps or unintended clipping |
| Desktop | Content width, hierarchy | Reading measure and spacing remain comfortable |
| Short viewport | Sticky headers, dialogs | Focused controls and primary actions are not obscured |
| 200% zoom | Reflow and text wrapping | Essential content remains available without two-dimensional scrolling where avoidable |
| Long content | Titles, validation, translated labels | Text wraps without overlap or truncation of meaning |

## Procedure
1. Start with the narrowest supported width and work upward.
2. Use realistic content, including long names and error messages.
3. Test at least one interactive state at each major layout transition.
4. Check orientation changes and browser zoom when relevant.
5. Record exact viewport dimensions and reproduction steps for defects.

Choose breakpoints based on where the content needs to change, not on a device-brand list.