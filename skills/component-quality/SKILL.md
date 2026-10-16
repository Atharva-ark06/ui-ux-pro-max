---
name: component-quality
description: Design or review reusable UI components with clear APIs, semantic behavior, predictable states, and practical tests.
---

# Component Quality

## Workflow
1. Define the user need and component responsibility.
2. Prefer native HTML semantics before adding custom behavior.
3. Keep the public API small and consistent with neighboring components.
4. Separate content, state, styling, and side effects clearly.
5. Include relevant hover, focus-visible, active, disabled, loading, error, and empty states.
6. Verify keyboard operation and accessible naming.
7. Consider responsive width, long content, localization, and zoom.
8. Add tests for behavior and edge cases, not snapshots alone.
9. Document intended use, constraints, and examples.
10. Check existing consumers for regressions.

## Review checklist
- [ ] One clear responsibility.
- [ ] Semantic HTML and accessible names.
- [ ] Stable, understandable props.
- [ ] Correct behavior when optional content is absent.
- [ ] Visible focus and keyboard support.
- [ ] Long text and narrow containers handled.
- [ ] Relevant loading, error, and disabled states.
- [ ] Tests cover important interactions and boundary cases.
- [ ] No unnecessary dependency or duplicated style logic.
- [ ] Examples match the current API.

## Avoid
- Props for hypothetical future needs.
- Clickable non-interactive elements without keyboard behavior.
- State changes hidden from assistive technology.
- New components when native elements or existing primitives suffice.
- Undocumented breaking changes.
