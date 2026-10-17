# Figma-to-Production UI Workflow

This workflow helps translate a Figma frame into maintainable UI code without treating a screenshot as the entire specification.

## Phase 1: Inspect the design

- Identify the target frame and copy its selection link.
- Ask the connected agent to inspect layout, spacing, typography, colors, variables, component instances, and responsive intent.
- Identify existing design-system components and code mappings before creating replacements.
- Note unknown states and interactions rather than guessing.

## Phase 2: Plan the implementation

- Map design elements to existing components.
- Identify reusable tokens for color, spacing, type, radius, and elevation.
- Decide which parts need responsive variants.
- List interaction states: hover, focus, disabled, loading, empty, and error.
- Confirm any missing behavior with the product owner or user.

## Phase 3: Implement incrementally

1. Build the page structure and semantic HTML.
2. Reuse existing components and tokens.
3. Add responsive behavior.
4. Implement keyboard interaction and visible focus.
5. Add loading, error, and empty states where relevant.
6. Avoid adding dependencies unless they solve a real requirement.

## Phase 4: Compare and verify

- Run the project's formatter, lint, type checks, and tests.
- Capture screenshots at the target viewport and at narrow/mobile widths.
- Compare spacing, typography, alignment, colors, and component states.
- Check keyboard-only navigation, labels, contrast, and reduced-motion behavior.
- Record visual differences and fix the highest-impact mismatches first.

## Phase 5: Review and deliver

The handoff should include the files changed, design decisions, verification performed, known gaps, and screenshots or preview links if available. Do not claim pixel-perfect parity without a comparison.

## Figma MCP references

- https://developers.figma.com/docs/figma-mcp-server/tools-and-prompts/
- https://developers.figma.com/docs/figma-mcp-server/
