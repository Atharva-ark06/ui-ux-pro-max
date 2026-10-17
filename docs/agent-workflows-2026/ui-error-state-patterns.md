# UI Error State Patterns

An error state should explain the impact and give the user a safe recovery path.

## Common categories
- Validation error: show what input needs correction.
- Network error: say whether retry is possible and preserve user work.
- Permission error: explain that access is unavailable without exposing sensitive details.
- Empty result: distinguish no data from a failed request.
- Unexpected error: provide a safe message and a support path where appropriate.

## Design principles
- Keep messages specific and actionable.
- Place the message near the affected task.
- Avoid exposing internal traces, tokens, or private system details.
- Preserve user input when safe.
- Prevent repeated submissions when an operation may have succeeded already.

## Testing
Simulate offline mode, timeouts, server errors, invalid input, expired sessions, and retry behavior. Confirm that errors are announced accessibly and do not trap keyboard users.