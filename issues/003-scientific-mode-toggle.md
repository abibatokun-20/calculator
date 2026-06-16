# Add advanced operations and scientific mode toggle

Description
- Add scientific functions (sin, cos, tan, power, sqrt, log) behind a toggleable "Scientific" mode.
- Persist the selected mode across sessions.

Motivation
- Provide advanced functionality for users who need more than basic arithmetic.

Acceptance criteria
- UI: A toggle to switch between Basic and Scientific modes; scientific buttons hidden in Basic.
- Functionality: Implement sin, cos, tan, pow, sqrt, log in the calculation engine.
- Persistence: Remember mode using localStorage or the same history/config JSON.
- Tests: Unit tests for each new operation and for mode persistence.

Tasks
- Extend `app.js` calculation engine with new functions.
- Update `index.html` with scientific buttons and a toggle control.
- Save mode preference and write tests for persistence and correctness.

Notes
- Consider using degrees/radians switch later; start with radians and document it.
