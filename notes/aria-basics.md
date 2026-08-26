# ARIA Basics

A quick scratchpad for accessible components.

## When to use ARIA
- Use native HTML elements first.
- Add ARIA only when HTML semantics are insufficient.
- Avoid redundant roles (e.g., `<button role="button">`).

## Common roles
- `dialog`: modal/non-modal dialogs.
- `alert`: live region for important messages.
- `navigation`: landmark for nav blocks.
- `main`: landmark for primary content.

## Live regions
- `aria-live="polite"` for updates users should notice soon.
- `aria-live="assertive"` for urgent updates (use sparingly).
- `aria-atomic="true"` if the entire region should be announced.

## Keyboard support
- Ensure all interactive elements are reachable via Tab.
- Use Enter/Space to activate buttons and links.
- Manage focus for dialogs: trap focus, return on close.

## Quick checks
- [ ] No `<div>` click handlers without keyboard support.
- [ ] Visible focus indicator is not removed.
- [ ] Color is not the only differentiator.
- [ ] Form errors are announced.
