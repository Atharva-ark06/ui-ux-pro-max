---
name: form-validation
description: Review form validation for understandable feedback, resilient input preservation, and secure handling.
---
# Form Validation
1. Validate data on the server even when client-side checks exist.
2. Explain constraints before submission where users need them.
3. Place inline errors near fields and associate them programmatically.
4. Preserve valid input and focus the first actionable error after failed submission.
5. Distinguish field errors from service-wide failures.
6. Do not reveal sensitive system details or account existence through error messages.
7. Avoid rejecting valid input due to unnecessary formatting assumptions.
8. Test boundary values, pasted input, keyboard-only submission, and network failures.
