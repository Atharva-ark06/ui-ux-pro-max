# Frontend Code Review Workflow

## Review order
1. Correctness and user-visible behavior
2. Security and privacy
3. Accessibility
4. Responsive behavior
5. Performance and rendering
6. Maintainability and consistency
7. Styling preferences

## Inspect
- Component state and effect dependencies
- Form validation and error recovery
- Keyboard interactions and semantic HTML
- API error handling and loading states
- Image sizing and layout shift
- Dependency and bundle changes
- Test coverage for edge cases

## Findings
Each finding should include a location, impact, scenario, and suggested fix. Avoid blocking a change over subjective style preferences when repository conventions already settle the question.

## Finish
Run relevant checks, inspect the final diff, and report what was actually tested.