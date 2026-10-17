# Repeatable Agent Workflow Patterns

These patterns help make coding-agent tasks predictable and reviewable.

## Pattern A: Understand before editing

1. Restate the requested outcome.
2. Inspect repository structure and relevant files.
3. Identify constraints, existing conventions, and missing information.
4. Propose a small plan.
5. Make focused changes only after the target is clear.

## Pattern B: Plan, implement, verify

1. Define acceptance criteria.
2. Implement the smallest coherent change.
3. Run relevant tests, lint, type checks, or manual verification.
4. Inspect the diff for unrelated edits and secrets.
5. Summarize results and remaining limitations.

## Pattern C: Design-to-code

1. Read the selected Figma frame and design tokens.
2. Map existing components before creating new ones.
3. Implement structure and responsive behavior.
4. Compare screenshots at agreed viewports.
5. Verify accessibility and interaction states.

## Pattern D: Review a pull request

1. Read the diff and surrounding code.
2. Prioritize correctness, security, data loss, regressions, and test gaps.
3. Cite file and line locations for findings.
4. Separate blocking issues from suggestions.
5. Avoid changing code while performing a review unless asked.

## Pattern E: Safe external action

Before publishing, deploying, deleting, or sending a message:
- Verify the exact target and scope.
- Check whether the user explicitly authorized the action.
- Explain irreversible effects when material.
- Request confirmation if authorization is ambiguous.
- Report the actual result, not an assumed success.

## Definition of done

A task is done when the requested outcome is delivered, relevant checks are run or their absence is disclosed, the diff is reviewed, and the handoff clearly states what changed.
