# Agent Skills Ecosystem: Practical Map

This guide maps reusable instruction packages across coding agents and design tools. It focuses on portable workflows rather than claiming every client uses an identical format.

## The common pattern

Most skill systems package a focused task into instructions plus optional examples, references, and scripts. A good skill states when it applies, defines a repeatable workflow, documents inputs and outputs, and includes checks for the result.

| Ecosystem | Common location / installation | Best use |
| --- | --- | --- |
| Claude Code | `.claude/skills/<name>/SKILL.md` for a project; `~/.claude/skills/<name>/SKILL.md` for a user | Reusable repository workflows and domain instructions |
| OpenAI Codex | `.agents/skills/<name>/SKILL.md` in a project or `~/.codex/skills/<name>/SKILL.md` for a user | Coding, review, planning, testing, and repeatable tasks |
| Figma MCP | Figma's official plugin/skills for supported clients | Design-context extraction, design-to-code, and canvas editing |
| MCP servers | Configured per client | Connect an agent to external tools and data sources |

Paths and available capabilities can vary by client version. Check the official documentation before installing or sharing a skill.

## A practical selection process

1. Define the repeated task and what a successful result looks like.
2. Search official or trusted skill sources first.
3. Read the entire `SKILL.md`, scripts, and referenced files before installing.
4. Check permissions, network use, dependencies, and whether commands modify files or external services.
5. Install at the narrowest scope that meets the need.
6. Test with a small, non-sensitive task.
7. Keep a short changelog and remove skills that are no longer maintained.

## Official starting points

- Claude Agent Skills: https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
- Codex skills: https://developers.openai.com/codex/skills/
- Codex repository: https://github.com/openai/codex
- Figma MCP: https://developers.figma.com/docs/figma-mcp-server/
- Agent Skills open standard: https://agentskills.io/

## Repository principle

A skill is a workflow asset, not proof of work by itself. Prefer maintained documentation, useful examples, and tested guidance over a large count of near-duplicate files.
