# Skill Authoring Checklist

Use this checklist when adding or revising a skill in this repository.

## Before writing
- [ ] Confirm the skill covers one coherent task.
- [ ] Choose a short, descriptive directory name.
- [ ] Check the existing catalog for overlap with another skill.
- [ ] Identify the intended user, trigger conditions, and expected output.

## Skill file
- [ ] Add a `SKILL.md` file with valid YAML frontmatter.
- [ ] Include a clear `name` and actionable `description`.
- [ ] State when to use the skill and when not to use it.
- [ ] Provide an ordered workflow with concrete decision points.
- [ ] Include failure cases, safety considerations, and verification steps.
- [ ] Prefer specific instructions over generic advice or unsupported claims.

## Examples and maintenance
- [ ] Add a concise example when it clarifies the expected result.
- [ ] Verify all relative links and referenced paths.
- [ ] Update `skills/README.md` with the correct link and summary.
- [ ] Review the result for duplication, stale references, and unnecessary dependencies.

## Final review
- [ ] Read the skill from the perspective of someone using it for the first time.
- [ ] Confirm the instructions produce a reviewable result.
- [ ] Summarize what changed and what was checked in the pull request.
