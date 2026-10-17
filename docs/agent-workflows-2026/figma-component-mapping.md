# Figma Component Mapping Workflow

Map design components to implementation components before generating new UI code.

## Mapping steps

1. Inspect the selected frame and identify component instances.
2. Find matching components in the codebase and design system.
3. Compare properties, variants, states, and responsive behavior.
4. Record exact matches, partial matches, and missing components.
5. Reuse exact matches where possible.
6. Extend a component only when the added behavior is coherent and backward-compatible.
7. Create a new component only when existing options do not fit.

## Mapping table

| Figma item | Code component | Match | Follow-up |
| --- | --- | --- | --- |
| Primary button | Existing Button | Exact / partial / none | Verify size and state variants |
| Navigation item | Existing NavLink | Exact / partial / none | Verify active and focus states |
| Card | Existing Card | Exact / partial / none | Check responsive layout |

## Validation

Check visual output at matching viewports, confirm semantic behavior, and update the mapping documentation when components change. Use Code Connect when supported and configured.

Reference: https://developers.figma.com/docs/figma-mcp-server/tools-and-prompts/
