# Motion and Animation Review

Motion can communicate relationships, but unnecessary movement can distract or cause discomfort.

## Review
- Does the animation communicate state or spatial continuity?
- Is duration appropriate to the interaction?
- Can users complete the task without waiting for decorative motion?
- Does the UI respect reduced-motion preferences?
- Do transitions avoid flashing and rapid repeated movement?
- Are layout shifts and performance costs controlled?

## Implementation
Prefer transform and opacity animations where appropriate, avoid animating large areas unnecessarily, and ensure state changes remain understandable when motion is reduced or unavailable.

## Verification
Test reduced-motion settings, keyboard focus during transitions, slower devices, and content changes. Keep essential information available without animation.