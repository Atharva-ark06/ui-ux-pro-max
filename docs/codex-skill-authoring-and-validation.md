# Codex Skill Authoring and Validation

## Recommended structure

```text
.agents/skills/<skill-name>/
  SKILL.md
  references/   # optional
  scripts/      # optional
  examples/     # optional
```

The `SKILL.md` should contain frontmatter with a name and a description that explains both capability and trigger conditions.

## Authoring workflow

1. Identify one repeated task, its inputs, and its expected output.
2. Write a concise description that distinguishes the skill from nearby skills.
3. Add numbered instructions in the order they should be followed.
4. Define when to ask a clarifying question and when to stop.
5. Specify validation commands or acceptance criteria.
6. Move bulky references into separate files and link to them.
7. Test trigger behavior, normal execution, incomplete inputs, and failure handling.

## Validation checklist

- [ ] Directory and skill name are consistent.
- [ ] Frontmatter is valid YAML and required fields are present.
- [ ] Description states both what the skill does and when it applies.
- [ ] Instructions are specific, ordered, and actionable.
- [ ] Referenced paths exist and use portable relative paths.
- [ ] Scripts are reviewed and do not expose secrets.
- [ ] No unrequested deployment, publishing, or destructive operation is implied.
- [ ] Expected output and verification steps are defined.
- [ ] At least one normal and one edge-case test has been completed.

## Keep skills composable

A code-review skill should review changes, not silently deploy them. A Figma skill should define design operations, not invent missing product requirements. Split workflows when permissions, audiences, or success criteria differ.

## Official resource

https://developers.openai.com/codex/skills/
