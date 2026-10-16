# Accessibility Smoke Test

Run this lightweight check on important flows before release. It complements, rather than replaces, assistive-technology testing and automated audits.

## Keyboard
- [ ] Reach every interactive element using Tab and Shift+Tab.
- [ ] Operate buttons, links, menus, and dialogs without a pointer.
- [ ] Confirm focus is clearly visible and follows a logical order.
- [ ] Confirm dialogs manage focus and return it to the invoking control when closed.

## Content and semantics
- [ ] Controls have accessible names that describe their purpose.
- [ ] Inputs have persistent labels and useful error descriptions.
- [ ] Headings communicate the page structure in order.
- [ ] Status updates are announced when necessary without stealing focus.

## Visual and motion
- [ ] Text and controls have sufficient contrast.
- [ ] Meaning is not communicated by color alone.
- [ ] Zoom and text resizing do not hide essential actions.
- [ ] Reduced-motion preferences avoid unnecessary animation.

Record the route, browser, assistive technology if used, steps, result, and unresolved barriers. Passing this checklist is not a claim of full WCAG conformance.