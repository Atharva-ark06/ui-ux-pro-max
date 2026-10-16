# Component API Review Guide

## Responsibility
- Does the component solve one coherent problem?
- Is a native element or existing component sufficient?
- Are behavior and presentation boundaries clear?

## API
- Are names consistent with neighboring components?
- Are defaults safe and predictable?
- Are invalid combinations prevented where possible?
- Are callbacks and controlled/uncontrolled states documented?

## Accessibility and states
- Are semantic roles and names correct?
- Is keyboard behavior predictable?
- Are focus, disabled, loading, error, and empty states defined?

## Compatibility
- Does optional content behave correctly when absent?
- Are long labels, localization, and narrow widths handled?
- Are breaking changes and migration steps documented?

## Evidence
- Are interaction tests included?
- Does the example use the current API?
- Were existing consumers checked for regressions?
