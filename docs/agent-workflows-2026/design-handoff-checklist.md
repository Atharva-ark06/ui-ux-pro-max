# Design Handoff Checklist

A useful handoff communicates behavior and constraints, not just appearance.

## Before handoff

- [ ] Link the source frame and identify target viewports.
- [ ] Use named components, variants, and variables.
- [ ] Include relevant loading, empty, error, disabled, and success states.
- [ ] Describe responsive behavior and content overflow.
- [ ] Specify keyboard, focus, and validation expectations.
- [ ] Provide realistic, non-sensitive sample content.

## Interaction details

For each interactive element, define the trigger, resulting state, feedback, and recovery path. Record behavior that cannot be inferred from static frames.

## Acceptance criteria

Write testable statements, such as:
- Primary actions remain usable at mobile widths.
- Invalid input shows a message associated with the field.
- Focus remains visible during keyboard navigation.
- Shared design tokens are used for typography and spacing.

The receiving developer should understand what to build, how it behaves, which components to reuse, and how it will be verified.
