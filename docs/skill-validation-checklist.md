# Skill Validation Checklist

Use this checklist to review a skill before merging it into the catalog.

## Structure
- [ ] The skill directory name is lowercase and descriptive.
- [ ] `SKILL.md` exists at the expected path.
- [ ] YAML frontmatter is valid and includes `name` and `description`.
- [ ] Headings and steps follow a logical order.

## Content quality
- [ ] The trigger conditions are specific enough to guide selection.
- [ ] Steps are actionable and can be followed in sequence.
- [ ] Inputs, assumptions, and expected outputs are stated.
- [ ] Important edge cases and failure paths are addressed.
- [ ] Security, privacy, accessibility, or reliability concerns are covered when relevant.
- [ ] Examples are consistent with the instructions and do not expose secrets.

## Links and catalog
- [ ] Relative links resolve from the skill's location.
- [ ] The catalog entry points to the correct `SKILL.md`.
- [ ] The catalog summary accurately describes the skill.
- [ ] No duplicate or conflicting skill entry was introduced.

## Review outcome
Record any blockers, the evidence checked, and follow-up work. A checklist pass is not a substitute for testing commands or code examples included in a skill.
