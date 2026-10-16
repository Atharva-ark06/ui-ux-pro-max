---
name: loading-states
description: Make waiting understandable through responsive feedback, progress indicators, and cancellation or recovery where appropriate.
---
# Loading States
1. Decide whether the operation is instant, delayed, long-running, or indeterminate.
2. Avoid flashing a spinner for operations that finish almost immediately.
3. Use skeletons only when they resemble the content being loaded.
4. Show meaningful progress only when the estimate is grounded in actual work.
5. Preserve layout dimensions to reduce visual shifts.
6. For long tasks, explain what is happening and offer cancel/retry when safe.
7. Announce important status changes accessibly without repeatedly interrupting screen readers.
Never invent percentages or promise a completion time that the system cannot support.
