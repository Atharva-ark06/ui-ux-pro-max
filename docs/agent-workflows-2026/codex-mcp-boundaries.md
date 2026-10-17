# Codex Skills and MCP Boundaries

A skill packages task instructions and optional resources. An MCP server exposes tools or context from an external service. A compatible client connects the two.

## Setup sequence

1. Verify client support and current documentation.
2. Install the skill in the documented scope.
3. Configure the MCP server separately.
4. Authenticate with the service provider.
5. Inspect available tools and permissions.
6. Test read-only access before write operations.

## Troubleshooting

If the skill is discovered but tools are missing, inspect the MCP connection. If tools are available but the workflow is inconsistent, review the skill. If neither works, verify client version, paths, authentication, and organization policy.

Do not assume a skill grants account access, or that a connected server makes every action safe.

References:
- https://developers.openai.com/codex/skills/
- https://developers.figma.com/docs/figma-mcp-server/
- https://modelcontextprotocol.io/
