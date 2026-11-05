# Command Center v4

Static, local-first task and routine manager. Deploy the **contents** of this folder at the root of the existing GitHub Pages repository. Do not upload the ZIP itself.

## Data preservation
Before upgrading, export a JSON backup from each v3 profile. V4 reads the same `command-center-v2` default profile and `command-center-profile-<id>` keys as v3, and adds a `v4` property in each profile's data. It does not require a server or account. Test on your original browser before importing anything.

## Features
Universal quick-add (`Ctrl/Cmd+J`), command palette (`Ctrl/Cmd+K`), natural-language task entry with today/tomorrow/next weekday and AM/PM times, trash/restore, per-profile theme/accent, dashboard widget visibility and ordering, task templates, weekday/after-completion recurrence, task dependencies, focus timer, individual-task calendar, profile-local productivity and custom goals, profile JSON export/import. Voice recognition remains browser-dependent.

## Important limits
Natural-language parsing is rule-based, not AI. Reminder toasts work only while the app is open. The focus timer runs while the page remains active; closing or reloading loses an unfinished session. Data remains in browser localStorage, not synchronized. Individual-profile backups are separate; export every profile. Productivity history predating v4 may lack granular completion events, so historical analytics are partial.

## Testing
JavaScript syntax validation is included in the build process. Full real-device/browser testing has not been completed.
