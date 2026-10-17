# Form UX and Validation Workflow

Good forms make the expected input clear and help users recover from mistakes.

## Design checklist
- Label every field and explain unusual requirements.
- Mark required fields consistently.
- Use appropriate input types and autocomplete hints.
- Validate at a useful time without interrupting every keystroke.
- Preserve valid input after errors.
- Place actionable error messages near the relevant field.
- Provide a clear success state and prevent accidental duplicate submissions.

## Implementation checks
- Validate on the server as well as in the browser.
- Treat client-side validation as usability, not a security boundary.
- Associate errors programmatically with their controls.
- Test keyboard use, screen-reader labels, invalid values, and network failures.

## Acceptance criteria
A user should understand what is required, identify an invalid field, correct it, and recover without re-entering unrelated data.