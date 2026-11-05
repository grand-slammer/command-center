## Command Center v4.2

Patch release: recurring tasks can now be given a final occurrence date (Repeat until). Calendar projections and generated future tasks respect that end date. Immersive Focus has a compact task selector and opposing teal/violet wave animation over black.

Existing local profile data is retained. Back up each profile before updating.

# Command Center v4.1 — incremental upgrade from v4

## Deploy without replacing your repository

1. **Export a JSON backup from every profile** in the current application.
2. Create a Git branch named `release/v4.1` from `main` (optional but recommended).
3. Update the existing files in your repository **in place**, preserving the same repository and URL. Commit as `feat: v4.1 smart add, recurring calendar, dashboard and focus`.
4. Test on the branch or locally, then merge to `main` to deploy. GitHub Pages can remain configured for `main` and root.
5. If anything goes wrong, use GitHub's commit history to revert the commit. Restoring a previous commit does not automatically restore browser data; keep backups.

## What's changed
- Smart Add opens a dedicated task-entry dialog from My Tasks or Ctrl/Cmd+K, with example commands and a preview.
- Dashboard widgets now render in saved order rather than only moving within the settings list.
- Upcoming recurring individual-task occurrences appear on the calendar, with a separate dashboard widget. Routine checklists remain excluded.
- Focus Mode adds optional immersive **Slow Waves** animated gradients, reduced motion, and a voluntary confirmation before exit. Browser fullscreen is requested where supported, but is not guaranteed on iPhone.
- Service-worker cache version updated so new files can replace v4 offline assets.

## Data and limitations
This build keeps the same localStorage profile keys and data format as v4; no data reset or import is intended. Recurring calendar entries are projections from saved due dates and repeat rules; they do not create separate stored tasks until an occurrence is completed through the existing recurrence flow. Browser-based strict focus cannot block other apps or system controls. Voice recognition and fullscreen vary by browser.

## Verification
JavaScript syntax and archive integrity were checked. Full browser interaction and iPhone testing are still required.
