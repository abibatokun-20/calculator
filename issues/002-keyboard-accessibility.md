# Add keyboard input and improve accessibility

Description
- Enable full keyboard control for the calculator (numbers, operators, Enter, Backspace, Escape).
- Improve accessibility with ARIA attributes, semantic HTML, and visible focus styles.

Motivation
- Keyboard users and screen-reader users should be able to use the calculator effectively.

Acceptance criteria
- Keyboard: Number keys and operator keys produce input; `Enter` evaluates; `Backspace` deletes; `Esc` clears.
- Accessibility: Buttons have `aria-label`s, appropriate `role` attributes, and are navigable via keyboard.
- Tests: Add automated tests for key handling and a basic a11y check (using axe or similar locally).

Tasks
- Update `index.html` to include ARIA attributes and logical tab order.
- Update `app.js` to add `keydown` handlers and focus management.
- Add CSS focus styles in `style.css`.
- Add tests for keyboard handling and document a11y improvements.

Notes
- Aim for WCAG AA compliance where practical.
