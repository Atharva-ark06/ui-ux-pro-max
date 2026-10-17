# Codex Code Review Skill Blueprint

Use this blueprint when creating a repository-specific review skill. Adapt it to the project's languages and test commands.

## Review sequence

1. Read the task, acceptance criteria, and complete diff.
2. Inspect surrounding code for contracts and conventions.
3. Prioritize correctness, security, data loss, compatibility, and regression risks.
4. Check input validation, error handling, permissions, and sensitive data handling.
5. Inspect tests and identify meaningful coverage gaps.
6. Report only actionable findings with file and line references.

## Finding format

For each confirmed issue include:
- Severity and concise title
- File and line range
- Scenario that triggers the problem
- Impact
- Suggested remediation

Do not report speculative issues as confirmed. Separate optional style suggestions from blocking defects.

## Validation

Test on a known-good change, a change containing a deliberate defect, and a change that should produce no findings. Confirm that the skill does not rewrite code unless explicitly asked.

Reference: https://developers.openai.com/codex/skills/
