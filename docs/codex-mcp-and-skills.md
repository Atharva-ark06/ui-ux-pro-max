# Codex Skills and MCP: How They Fit Together

A skill and an MCP server are complementary, not interchangeable.

- **Skill:** instructions and supporting resources that describe how to complete a task.
- **MCP server:** a connection that exposes tools or context from an external service.
- **Client:** the agent application that discovers skills and manages tool access.

For example, a Figma skill can explain how to inspect a frame, reuse design tokens, and verify a generated UI. The Figma MCP connection supplies the actual design tools.

## Setup sequence

1. Confirm the client supports the desired skill format and MCP transport.
2. Install or add the skill using the documented method.
3. Configure the MCP server through the client.
4. Authenticate with the provider.
5. Inspect available tools and permissions.
6. Test a read-only request.
7. Test write operations only in a draft or approved workspace.

## Troubleshooting

If a skill is recognized but tools are missing, check the MCP connection. If tools work but the workflow is poor, review the skill instructions. If neither is available, verify client version, paths, authentication, and organization policy.

## Safety boundary

Do not assume that installing a skill grants service access. Do not assume that connecting a server makes every operation safe. Review both instructions and permissions.

## Official references

https://developers.openai.com/codex/skills/
https://developers.figma.com/docs/figma-mcp-server/
https://modelcontextprotocol.io/
