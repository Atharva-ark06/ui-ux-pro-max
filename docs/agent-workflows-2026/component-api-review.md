# Component API Review Checklist

A component API should be predictable, accessible, and easy to reuse.

## Review questions
- Are prop names clear and consistent with neighboring components?
- Are required and optional props justified?
- Are variants limited to meaningful visual or behavioral differences?
- Are callbacks named for the event they represent?
- Are loading, disabled, error, and empty states defined where relevant?
- Can consumers provide accessible labels and content?
- Are defaults safe and unsurprising?

## Engineering
Avoid boolean-prop combinations that create ambiguous states. Prefer composition when a component has many unrelated responsibilities. Document breaking changes and update usage examples.

## Tests
Cover the default state, important variants, keyboard behavior, error cases, and backwards compatibility when the component is shared widely.