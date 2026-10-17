# MCP Server Selection Guide

The Model Context Protocol (MCP) provides a standard way for compatible clients to connect to external tools and context sources. A server exposes tools or resources; the client decides how to present and invoke them.

## When to use MCP

Use MCP when an agent needs structured access to a service that is not already available in its current context—for example, design files, issue trackers, or approved data sources.

## Remote versus local

| Mode | Benefits | Considerations |
| --- | --- | --- |
| Remote hosted server | No local service to maintain; provider handles hosting | Account authorization, provider access, network availability |
| Local desktop/server | Can integrate with local applications or local resources | Requires the app/service to run; local configuration and permissions matter |

Prefer the provider's official connection method and least-privilege authorization.

## Safe setup sequence

1. Verify the server's official documentation and endpoint.
2. Check the supported client/version.
3. Review the scopes requested during authentication.
4. Add the server using the client's documented configuration.
5. Authenticate in the provider's own sign-in flow.
6. Inspect the tools exposed by the server.
7. Test a read-only request first.
8. Only then test write operations in a safe draft or test workspace.

## Troubleshooting

- Confirm the client supports the server's transport and authentication.
- Restart or refresh the client if newly added tools are missing.
- Re-authenticate if access expires.
- Check organization policies and seat/plan requirements.
- Avoid copying access tokens into source files or shared logs.

## Figma example

Figma's remote MCP endpoint is `https://mcp.figma.com/mcp`. Use the official Figma guide for exact client setup and current capabilities.

https://modelcontextprotocol.io/
https://developers.figma.com/docs/figma-mcp-server/
