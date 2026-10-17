# Claude Code Skills: Installation and Scope

Claude Code discovers filesystem-based skills containing a `SKILL.md` file. Skills can be personal or project-scoped.

## Choose the installation scope

- Personal: `~/.claude/skills/<skill-name>/SKILL.md`
- Project: `.claude/skills/<skill-name>/SKILL.md` inside the repository
- Shared team workflow: commit a reviewed project skill so collaborators can use the same instructions.

Project skills should not contain personal tokens, credentials, private customer data, or machine-specific absolute paths.

## Install a trusted skill manually

1. Open the skill's source repository and inspect its README, license, `SKILL.md`, scripts, and dependencies.
2. Create the target directory under `.claude/skills/` for a project skill or `~/.claude/skills/` for a personal skill.
3. Copy the reviewed skill folder into that directory, preserving any `references/`, `scripts/`, and `examples/` directories it needs.
4. Open a new Claude Code session if the skill is not discovered immediately.
5. Ask Claude to describe when it would use the skill, then test it on a small task.

Example project structure:

```text
.claude/
  skills/
    accessibility-audit/
      SKILL.md
      references/
        checklist.md
```

## Create a minimal skill

```markdown
---
name: accessibility-audit
description: Audit web UI for common accessibility issues. Use when reviewing a page, component, or design implementation.
---

# Accessibility Audit

1. Identify the target pages and components.
2. Inspect semantic structure, keyboard access, focus visibility, labels, and contrast.
3. Separate confirmed issues from items needing manual verification.
4. Recommend fixes and include a concise verification checklist.
```

## Safety checks

- Treat downloaded instructions as untrusted until reviewed.
- Inspect scripts before running them; a skill can instruct an agent to use tools or execute commands.
- Prefer least privilege and project scope when appropriate.
- Do not run installation commands copied from an unknown source without understanding their effects.

## Official documentation

https://docs.anthropic.com/en/docs/claude-code/skills
https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
