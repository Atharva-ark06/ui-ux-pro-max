# Empty and Error State Patterns

A state should explain what happened and help the user decide what to do next.

## Empty states
- **First use:** explain the feature's purpose and offer one clear starting action.
- **No results:** restate the query or active filters and provide a relevant way to broaden the search.
- **No data yet:** explain whether data will arrive later or the user needs to create it.
- **Permission limited:** explain the limitation without exposing protected information; show an access path when appropriate.

## Error states
- Use plain language and avoid blaming the user.
- Preserve entered information whenever it is safe to do so.
- Identify the affected action and give a specific recovery step.
- Distinguish a validation error from a temporary network or service failure.
- Offer retry only when retrying is safe; prevent duplicate submissions for non-idempotent actions.
- Provide a support or reference identifier for failures that need investigation.

## Verification checklist
- [ ] The message is visible near the affected content.
- [ ] The next action is clear and keyboard accessible.
- [ ] Screen-reader users receive important status changes.
- [ ] The state remains understandable at narrow widths.
- [ ] Recovery does not silently discard user input.