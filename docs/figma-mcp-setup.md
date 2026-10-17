# Figma MCP: Setup and First Connection

The Figma MCP server lets supported AI clients read design context from Figma. Depending on client, plan, and server mode, it may also support writing native content to the canvas.

## Recommended: remote server

Figma documents the remote endpoint as:

```text
https://mcp.figma.com/mcp
```

The remote server does not require the Figma desktop app. Connect using a supported client and complete the Figma sign-in/authorization flow.

## Claude Code

Figma's documented plugin installation command is:

```powershell
claude plugin install figma@claude-plugins-official
```

Restart Claude Code, open `/plugin`, locate the installed Figma plugin, and complete the sign-in flow. If plugin installation is unavailable, consult Figma's manual MCP setup instructions.

## Other supported clients

Use the current Figma setup page for Codex, Cursor, VS Code, and other listed clients. Prefer an official client plugin where available because it can include both MCP configuration and Figma-specific skills.

## First test

1. Open a Figma file and copy a link to a specific frame or layer.
2. Give that link to the connected agent.
3. Ask it to summarize the layout, components, variables, and design constraints.
4. Compare the summary with the actual design before asking for code changes.
5. For write-to-canvas workflows, begin with a new draft or duplicate and review the proposed changes before relying on them.

## Permissions and plan notes

Figma capabilities differ by plan, seat, client, and remote versus desktop server. Writing to files outside drafts may require a Full seat. Confirm current plan details before depending on write operations.

## Official docs

- https://developers.figma.com/docs/figma-mcp-server/
- https://developers.figma.com/docs/figma-mcp-server/remote-server-installation/
- https://developers.figma.com/docs/figma-mcp-server/tools-and-prompts/
