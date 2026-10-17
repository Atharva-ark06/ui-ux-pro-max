# Figma Agent Prompt Recipes

Use these prompts with a client that has been connected to Figma MCP. Include a link to the target frame or layer when applicable.

## Inspect a design

> Inspect this Figma frame and summarize its layout, typography, color variables, spacing, component instances, and responsive assumptions. Separate observed facts from assumptions. Do not edit the file yet.

## Implement a frame in an existing codebase

> Use this Figma selection as the source of truth. First inspect the repository and identify existing components and design tokens. Propose a mapping from Figma elements to existing code, then implement the smallest coherent change. Preserve accessibility and responsive behavior. Run relevant checks and report any visual differences.

## Audit accessibility

> Review this design for keyboard and focus requirements, semantic structure, text contrast, target size, labels, error states, and reduced-motion needs. Distinguish issues visible in the design from issues that require browser testing.

## Create a component proposal

> Identify repeated patterns in this file and propose a component/variant structure. Reuse existing library components and variables where possible. Do not change the source file until I approve the proposal.

## Compare implementation with design

> Compare the running UI with the linked Figma frame at the same viewport. List the highest-impact differences in order: geometry, typography, color, component states, and responsive behavior. Do not claim pixel-perfect parity without evidence.

## Create or edit Figma content

> In a new draft or approved target file, create the requested frames using existing components and variables where possible. Summarize what you changed and provide the resulting Figma link. Ask before overwriting existing design content.

## Good prompt hygiene

- Name the target frame and intended outcome.
- Provide viewport and framework constraints.
- State whether the agent may edit code, Figma, or both.
- Require a diff or summary and validation.
- Explicitly prohibit publishing or destructive actions when they are out of scope.

Figma MCP reference: https://developers.figma.com/docs/figma-mcp-server/tools-and-prompts/
