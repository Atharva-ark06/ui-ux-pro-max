# Design Token Governance

Design tokens keep visual decisions consistent across components and themes.

## Token layers

- Primitive: raw color, spacing, type, radius, and elevation values.
- Semantic: purpose-based values such as `text-primary`, `surface-muted`, and `border-focus`.
- Component: values needed by a specific component when semantic tokens are insufficient.

Prefer semantic tokens in product UI so themes can evolve without changing every component.

## Change workflow

1. Search for an existing token before adding one.
2. Check contrast and light/dark theme behavior.
3. Update design and code mappings together where practical.
4. Find consumers before renaming or removing a token.
5. Run visual regression checks.
6. Document migrations for breaking changes.

## Review checklist

- [ ] Purpose and naming are clear.
- [ ] Existing tokens were considered.
- [ ] Theme and contrast implications were checked.
- [ ] Consumers and migration impact are understood.
- [ ] Design and implementation remain aligned.
