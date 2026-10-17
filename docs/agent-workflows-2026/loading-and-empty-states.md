# Loading and Empty State Patterns

Loading and empty states should communicate what is happening without making the interface feel broken.

## Loading
- Show feedback when a request takes noticeable time.
- Preserve context during refreshes where possible.
- Use skeletons only when they improve perceived structure.
- Avoid indefinite spinners without a recovery or timeout path.
- Prevent duplicate actions when the operation is in progress.

## Empty
Distinguish first-use, no search results, filtered-to-zero, and genuinely unavailable data. Explain the reason and offer a relevant next action.

## Verification
Test slow networks, empty API responses, filters that return no results, failed requests, and retry behavior. Ensure loading indicators do not cause major layout shifts or block unrelated interactions.