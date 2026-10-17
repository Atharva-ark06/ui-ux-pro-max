# Maintaining and Versioning Agent Skills

Skills are small pieces of workflow infrastructure. Treat them like code: review changes, preserve provenance, and test behavior.

## Recommended metadata

For each adopted external skill, record:
- Skill name and intended purpose
- Upstream repository and source path
- License
- Date reviewed
- Known dependencies
- Supported client(s)
- Local changes, if any

## Update process

1. Read the upstream changelog or diff.
2. Review changes to instructions and scripts.
3. Re-run the security checklist.
4. Test the normal workflow and at least one edge case.
5. Update local documentation and source metadata.
6. Commit the reviewed update with a specific message.

## Naming and scope

Use names that describe a task, such as `figma-design-to-code` or `secure-pr-review`. Avoid generic names such as `helper` or `everything`.

Keep a skill project-scoped when teammates need the same workflow. Use personal scope for private preferences or local experiments. Do not commit credentials or machine-specific configuration.

## Deprecation

Mark a skill as deprecated when its source is unmaintained, its workflow no longer matches current tooling, or a better-supported alternative replaces it. Include a migration note and remove it after consumers have moved.

## Related guides

- [Agent skills ecosystem](agent-skills-ecosystem.md)
- [Security review](agent-skill-security-review.md)
- [Quality rubric](agent-skill-quality-rubric.md)
