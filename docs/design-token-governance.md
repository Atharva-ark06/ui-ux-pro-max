# Design Token Governance

Design tokens make repeated decisions explicit and help interfaces stay consistent as products grow.

## Token structure
- Use semantic names such as `text-primary`, `surface-raised`, and `border-subtle` instead of naming tokens only by color value.
- Separate primitive values from semantic roles so themes can change without rewriting components.
- Define typography, spacing, radius, elevation, and motion tokens alongside color.
- Document supported themes and contrast expectations for each semantic role.

## Change workflow
1. Search for current token usage and identify affected components.
2. Propose the semantic change with before/after examples.
3. Check contrast, focus indicators, disabled states, and data visualization colors.
4. Preview representative screens and themes.
5. Update examples and document any intentional exception.

Avoid adding a token for a one-off value unless it represents a reusable design decision. Remove obsolete tokens only after checking consumers.