# MCP Authentication Review


Use the provider's supported authentication flow. Prefer scoped access and short-lived credentials when available. Never commit access tokens, client secrets, or private configuration values.

Check where tokens are stored, how consent is granted, what scopes are requested, how access can be revoked, and what happens after token expiry. Treat logs and tool output as potential sensitive-data surfaces.

Reference: https://modelcontextprotocol.io/
