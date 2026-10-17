# Product Requirements to Tests

Turn a product request into verifiable behavior before implementation begins.

## Requirement decomposition

For each requirement, identify:
- Actor and goal
- Preconditions
- Primary success path
- Validation and error cases
- Permissions and privacy constraints
- Empty, loading, and recovery states
- Observable acceptance criteria

## Example

Requirement: a user can update a profile display name.

Possible checks:
- A valid name is saved and shown after reload.
- Empty or over-limit values receive clear validation.
- An unauthorized user cannot update another account.
- A failed request preserves the previous value and explains recovery.
- Keyboard users can complete the flow.

## Test mapping

Map each acceptance criterion to a unit, integration, end-to-end, accessibility, or manual test. Avoid writing tests that only repeat implementation details.

## Review

Ask whether the tests would catch a realistic failure. Record requirements that remain ambiguous instead of silently inventing behavior.
