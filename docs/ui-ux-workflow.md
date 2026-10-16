# UI/UX Delivery Workflow

Adapt this workflow to project size and risk; not every change needs heavyweight ceremony.

## 1. Understand the problem
- Identify users, their primary task, and the context of use.
- Record platform, framework, brand, content, deadline, and accessibility constraints.
- Define success criteria and how they will be checked.

## 2. Structure the experience
- List required content and actions.
- Group information by user priority.
- Map the main path and important failure/recovery paths.
- Sketch the information hierarchy before fine visual styling.

## 3. Define visual rules
- Establish semantic color roles, typography, spacing, and shape.
- Choose a visual direction suited to the product and audience.
- Specify reusable patterns for navigation, forms, buttons, alerts, and empty states.
- Document justified exceptions.

## 4. Implement incrementally
- Reuse project conventions and components.
- Build the smallest coherent vertical slice first.
- Keep content, presentation, and behavior understandable.
- Avoid dependencies without a clear benefit.

## 5. Validate the experience
- Test keyboard-only navigation and visible focus.
- Check text and interface contrast.
- Inspect responsive layouts around breakpoints.
- Test empty, loading, error, disabled, and success states.
- Use realistic content, including long labels and validation messages.
- Run available lint, type, test, and build commands.

## 6. Review and ship
- Compare the result against acceptance criteria.
- Record known limitations rather than implying untested guarantees.
- Summarize changes, checks performed, and follow-up work.
- Ask a representative user to complete the primary task when practical.

## Definition of done
- The primary task is clear and works.
- Content remains readable at supported widths.
- Keyboard users can reach and operate controls.
- Feedback and error states are understandable.
- Shared patterns remain consistent.
- Available checks pass or failures are documented.
