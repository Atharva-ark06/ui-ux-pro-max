---
name: error-recovery
description: Design errors that explain what happened, what the user can do, and how to recover safely.
---
# Error Recovery
1. Identify whether the cause is user input, permissions, connectivity, server failure, or an unknown condition.
2. Explain the problem in plain language without exposing secrets or internal stack traces.
3. State the impact: was the action saved, partially completed, or not completed?
4. Offer a safe next action such as retry, edit, sign in, or contact support.
5. Preserve entered data when possible and prevent accidental duplicate submissions.
6. Include a stable reference identifier for support when appropriate.
7. Test repeated failures, offline recovery, expired sessions, and retry behavior.
Do not blame the user or present an unverified guess as the cause.
