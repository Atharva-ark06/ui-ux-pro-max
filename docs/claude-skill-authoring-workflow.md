# Authoring a Reliable Claude Code Skill

## 1. Define the trigger

Write a description that says both what the skill does and when it should be used. Keep the task narrow enough that the workflow can be followed consistently.

## 2. Use the standard structure

```text
skill-name/
  SKILL.md
  references/   # optional detailed guidance
  scripts/      # optional reviewed helper scripts
  examples/     # optional input/output examples
```

A `SKILL.md` begins with YAML frontmatter. Use a lowercase, hyphenated `name` and a useful `description`. Check current Claude Code documentation for the exact metadata constraints.

## 3. Write an executable workflow

A useful skill tells the agent to:
1. Confirm the task and required inputs.
2. Inspect the relevant project files before changing anything.
3. Follow a clear sequence of actions.
4. Respect scope, permissions, and existing conventions.
5. Validate the output and report unresolved assumptions.

Avoid vague instructions such as “make it perfect.” Define observable checks.

## 4. Keep context lean

Put the essential workflow in `SKILL.md`. Move long references, domain-specific examples, or troubleshooting notes into separate files and link to them explicitly. Avoid repeating the same rules across multiple skills.

## 5. Test with representative tasks

- A normal task that should trigger the skill.
- A similar task that should not trigger it.
- An incomplete-input task.
- A task that would modify files or use external tools.
- A task with an ambiguous or unsafe request.

Record whether the skill triggered appropriately, followed the sequence, and produced verifiable output.

## 6. Maintain it

Version changes in Git, include a concise changelog when useful, and update examples when the underlying tool changes. Prefer a small focused skill over one enormous “do everything” skill.

## References

- https://docs.anthropic.com/en/docs/claude-code/skills
- https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
