# Figma Variable Audit Checklist

## Inventory
- Identify variable collections, modes, names, and consumers.
- Find repeated raw values that should use shared tokens.
- Find duplicate variables with unclear differences.
- Check naming consistency and semantic purpose.

## Theme and mode checks
- Verify that each required mode has a value.
- Check contrast and state colors across modes.
- Identify components that bypass variables with hard-coded values.
- Confirm variable aliases do not create confusing dependencies.

## Change safety
Before renaming or deleting a variable, identify consumers and migration impact. Use a duplicate or draft for risky experiments and validate representative components after changes.

## Handoff
Record the variable, issue, affected components, recommended change, and verification method. Do not claim a full audit from a partial page or limited selection.

Figma MCP reference: https://developers.figma.com/docs/figma-mcp-server/