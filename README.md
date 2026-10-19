# Escape the Evil AI

A short branching text adventure played through browser prompts, alerts, confirmation dialogs, and the browser console. Explore the Control Room, Security Archive, Reactor Room, and Exit Gate. The keycard and security-grid state persist when revisiting rooms. Escaping requires both the keycard and a disabled security grid; attempting the gate without both leads to an unsuccessful ending.

## Run
1. Open `index.html` in a modern browser.
2. Read the opening alert before playing.
3. Keep the browser Console open to follow story events. In Chrome on Windows/Linux, press `Ctrl+Shift+J` or `F12` and select **Console**. On macOS, press `Cmd+Option+J`.
4. Enter one of the exact action words shown in each prompt. Capitalization and surrounding spaces are accepted. Invalid input changes nothing. Press **Cancel** in a choice prompt to end the run safely.
5. At the end, choose **OK** in the confirmation dialog to restart with a fresh state, or **Cancel** to finish.

## Suggested path to the successful ending
1. Control Room → `archive` → `take` to collect the keycard.
2. Security Archive → `reactor` → `disable` to disable the security grid.
3. Reactor Room → `control` → `exit` → `use` to escape.

Trying `use` at the Exit Gate before collecting both requirements demonstrates the unsuccessful ending.

## Files
- `index.html`: blank page boilerplate that loads the external script.
- `script.js`: story, state, validation, navigation, endings, and replay logic.

No CSS, DOM manipulation, dependencies, or build step are used.
