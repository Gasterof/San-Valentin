# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Interactive Valentine's Day webpage (in Spanish) that asks "Would you be my Valentine?" with playful button behavior. Built with vanilla HTML, CSS, and JavaScript — no build tools, frameworks, or package manager.

## Running the Project

Open `index.html` directly in a browser, or use VS Code Live Server (configured on port 5501 in `.vscode/settings.json`).

## Architecture

**Single-page app with three files:**

- `index.html` — Minimal markup: a container with a heading, message paragraphs, "Yes"/"No" buttons, an image container, and a dark mode toggle.
- `script.js` — All interactivity via vanilla DOM manipulation:
  - **"Yes" button**: Clears the container and replaces it with a 6-image Snoopy grid (external URLs) and a love message. Uses `container.innerHTML = ''` to wipe and rebuild the DOM.
  - **"No" button**: On first click, scales the button with a CSS transition. On subsequent clicks and hovers, the button repositions randomly across the viewport using `position: fixed` with random coordinates. Also shows a teasing message.
  - **Dark mode toggle**: Toggles `dark-mode` class on `<body>`.
- `styles.css` — Responsive layout with flexbox. Image grid uses `calc()` for 2-column mobile / 3-column desktop (`@media min-width: 768px`). Dark mode styles use `body.dark-mode` selector. CSS animations: `fadeIn` for the grid, `slideIn` for the response message.

## Key Behavior Details

- The "No" button's `mouseover` listener is only attached after the first click (via `mouseoverNoButton()` called inside the click handler), so hover-dodge only activates after clicking "No" once.
- Clicking "Yes" completely destroys and rebuilds the container's inner DOM — any references to original elements (buttons, response paragraph) become stale after this.
- Images in the "Yes" gallery are hardcoded external URLs (fineartamerica.com, dtfdallas.com, pinimg.com). The "No" hover image references an iCloud link.
