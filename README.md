# NicLog
A local-first, installable PWA to record vaping sessions or individual puffs. No backend, dependencies, or accounts.

## Deploy (GitHub Pages)
1. Create an empty public GitHub repository, e.g. `niclog`.
2. Upload the contents of this folder (not the folder itself) to the `main` branch.
3. Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
4. Open the published HTTPS address in Safari on your iPhone. Share → Add to Home Screen → Open as Web App (if offered) → Add.
5. Open the installed app online once. Settings will report when offline access is ready. Then use that same installed app for logging.

## Local test
Run `python3 -m http.server 8000` from this directory and visit http://localhost:8000. Offline support requires HTTPS or localhost.

## Privacy and data
Usage records stay in the web app's local storage. Hosting serves only static files. Storage can be cleared by the browser or OS, and Safari and the installed web app may not share storage. Export JSON backups regularly; use Import JSON backup to merge entries by ID. CSV is for analysis, not restoration. Session and puff entries are separate counts, not estimates of nicotine intake. No background logging, native widgets or Action Button integration is included in this release.
