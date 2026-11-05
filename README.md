# Command Center v3 — Local profiles

Adds a **Profile** selector and **+ Profile** button to v2. Each profile has its own tasks, routine templates, runs, calendar, history, and theme. Switching profiles reloads the view with that profile’s local data.

## Deploy

1. Export a backup from your current v2 site first.
2. Unzip this package and upload **the files inside the folder** to the root of your existing GitHub repository. Replace the old files with matching names.
3. Commit changes and refresh the GitHub Pages website.

## Storage and safety

- The existing v2 data remains the **Personal** profile, stored under the original `command-center-v2` key.
- New profiles get separate localStorage keys. They start with default example routines, but no task history.
- Each profile has its own export/import via Settings; switching does not merge lists.
- Profiles are **not password-protected** and are only available in the same browser on the same device. They do not sync across devices.
- Do not clear browser site data without exporting backups from each profile.
- Existing v2 features are retained, including a calendar showing only standalone tasks.
