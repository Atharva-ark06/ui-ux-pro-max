# Drafting Release Notes from Pull Requests

Release notes should describe user and operator impact, not merely repeat commit subjects.

## Workflow
1. Gather merged PR titles, descriptions, and labels for the release range.
2. Read the changes for context; do not infer behavior from titles alone.
3. Group changes into features, fixes, security, performance, and breaking changes.
4. Explain impact in plain language.
5. Identify required migration steps and known limitations.
6. Verify version numbers and links.
7. Have an owner review the draft before publication.

## Quality checks
- Avoid claiming a bug is fixed without evidence.
- Do not include secrets or private incident details.
- Keep internal refactoring separate from user-visible features.
- Link to relevant PRs or docs.
- Label breaking changes clearly.

This workflow drafts notes; publishing them is a separate action requiring authorization.