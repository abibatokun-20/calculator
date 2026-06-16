# Add persistent calculation history

Description
- Add a calculation history that records each operation and result.
- Persist history to a local JSON file (`history.json`) so it survives restarts.

Motivation
- Users should be able to review past calculations and reuse results.

Acceptance criteria
- Saving: Each completed calculation is appended to `history.json`.
- Loading: App loads history on startup and displays it in the UI.
- UI: Add a history view with options to clear or export history.
- Tests: Unit tests for save/load and for history trimming when file becomes large.

Tasks
- Update `app.js` to record operations and expose `saveHistory()` / `loadHistory()`.
- Add a history panel to `index.html` and styles in `style.css`.
- Add unit tests for persistence logic.
- Document new behavior in README.

Notes
- Use a simple JSON array of objects: `{ "id": 1, "expr": "2+2", "result": 4, "ts": 162... }`.
- Keep the format stable for future migrations.
