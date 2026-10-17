# OpenAI Codex Skills: Installation Guide

Codex skills package instructions and optional resources into reusable directories. A skill typically contains a `SKILL.md` with frontmatter and workflow instructions.

## Common locations

- Project-level: `.agents/skills/<skill-name>/SKILL.md`
- User-level: `~/.codex/skills/<skill-name>/SKILL.md`

Use the current Codex documentation for version-specific behavior and discovery rules.

## Install a skill

### Option A: Use the skill installer

In Codex, ask the built-in `$skill-installer` to list available skills or install a named curated skill. For a repository skill, provide its GitHub directory URL when supported.

Examples of the kind of request to make inside Codex:

```text
$skill-installer list available curated skills
$skill-installer install the <skill-name> skill
```

The exact supported command phrasing depends on the installed installer skill. Follow its instructions rather than assuming every version accepts identical arguments.

### Option B: Add a reviewed skill to a project

1. Inspect the source and license.
2. Copy the complete skill directory to `.agents/skills/<skill-name>/`.
3. Confirm that `SKILL.md` and any referenced resources are present.
4. Start a new Codex session if needed.
5. Test it on a small task and inspect the resulting changes.

Example:

```text
.agents/
  skills/
    pr-review/
      SKILL.md
      references/
        review-checklist.md
```

## Example frontmatter

```yaml
---
name: pr-review
description: Review a proposed code change for correctness, security, regressions, and test gaps. Use when reviewing a pull request or diff.
---
```

## Security and maintenance

- Review shell commands and scripts before executing them.
- Do not store API keys or private data in a skill.
- Keep write operations and external actions within the user's requested scope.
- Prefer skills with clear ownership, licenses, and testable outputs.
- Restart or start a new Codex session if an installed skill is not recognized.

## Official resources

- https://developers.openai.com/codex/skills/
- https://github.com/openai/codex
- https://github.com/openai/skills (check its current README and deprecation notices before relying on it)
