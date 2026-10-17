# Cross-Client Skill Migration Guide

A skill written for one agent may need adaptation before another client can use it reliably.

## Migration checklist

1. Identify the source client and target client.
2. Check each client's skill discovery path and frontmatter requirements.
3. Separate portable task instructions from client-specific commands.
4. Replace unsupported tool names with the target client's documented equivalents.
5. Re-check paths, environment assumptions, and shell syntax.
6. Review permissions and side effects.
7. Test positive and negative triggers.
8. Document features that cannot be migrated.

## Keep portable instructions portable

Prefer plain, ordered workflow steps and relative references. Put client-specific installation and tool invocation details in a separate section or adapter skill.

## Do not assume equivalence

A shared `SKILL.md` format does not guarantee identical discovery, context loading, tools, approvals, or runtime behavior. Verify the target client rather than copying the folder and assuming success.

References:
- https://agentskills.io/
- https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
- https://developers.openai.com/codex/skills/
