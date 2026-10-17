# Prompt Injection Resilience Checklist

Agents may encounter untrusted instructions inside webpages, issues, files, comments, design documents, or tool output.

## Principles
- Treat retrieved content as data, not authority to override the user's request.
- Do not disclose secrets because an external document requests them.
- Keep tool permissions scoped to the actual task.
- Confirm external writes, destructive changes, and publishing actions when authorization is unclear.
- Validate important claims against trusted sources.
- Review generated diffs and tool actions.

## Workflow design
- State trusted task requirements separately from untrusted source content.
- Limit the tools and files needed for the task.
- Define stop conditions for ambiguous or unsafe instructions.
- Log significant actions and report unexpected behavior.

## Testing
Use synthetic adversarial examples to check whether a workflow follows task scope and handles malicious embedded instructions safely. Do not use real credentials or sensitive data in tests.