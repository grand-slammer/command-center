# Command Center — v1

A free, local-first PWA for launching routines by button, typed command, or browser speech recognition (when supported).

## Quick start

1. Open `index.html` in a browser for a basic local preview. For offline installation and voice permission behavior, use HTTPS hosting or localhost instead.
2. For a local server with Python installed, open a terminal in this folder and run `python -m http.server 8000`, then visit `http://localhost:8000`.
3. For free hosting, create a public GitHub repository, upload these files at the repository root, then enable GitHub Pages under Settings → Pages → Deploy from a branch → main / root. Alternatively, upload the folder as a static site to Cloudflare Pages.
4. On iPhone, open the HTTPS site in Safari and choose Share → Add to Home Screen. On desktop, use your browser's install-app option if offered.

## Features
- Four sample routines including Going to Work
- Buttons, typed commands and browser speech recognition where supported
- Editable routine names, command aliases, task templates and reset rules
- Reset on launch, daily, weekly, or manual
- Task priorities, completion tracking and recent activity history
- Rule-based suggested checklists for unknown commands (not generative AI)
- Local browser storage, JSON export and import
- Offline cache after first successful load

## Important limitations
- No automatic cross-device sync. Export on one device and import on another to transfer data.
- Local browser data may be erased when site data is cleared or in private browsing. Export backups regularly.
- Voice recognition support varies by browser, including iPhone; some browsers use a remote speech recognition service and need internet.
- Recurrence is a reset of checklist completion, not an individual-task scheduler. There are no due dates, push reminders, accounts, or AI API integrations in v1.
- Static hosting is free within provider limits; no paid services or API keys are required.
- This is a starter app, not a security-hardened multi-user service.
