# ShiftSheet

ShiftSheet is a phone-friendly first version of a hockey stats tracker for volunteer teams. It is a Progressive Web App (PWA), so it can be added to an iPhone Home Screen without submitting an App Store app.

## What it does

- Set up your team name, opponent, and game date.
- Add players by jersey number and name, then log an event by choosing an event button and tapping a player.
- Turn preset events on and off. Presets include goals, assists, shots on goal, missed shots, blocked shots, saves, completed passes, takeaways, and penalties.
- Create and remove custom events. Custom events are counted in player and season totals.
- Track periods, team and opponent goals, review or undo recent events, and save a finished game.
- View season totals, share a text game summary, or export the full event list as CSV.
- Export a season report through the browser's print dialog and save/print it as PDF.
- Export player totals and the detailed event log as separate CSV files that open in Excel, Numbers, or Google Sheets.
- Keep working offline after the app has first loaded from a secure website.

## Put it on an iPhone

These files are a static website. To install it like an app, publish the contents of this folder to any HTTPS static host, then open its `index.html` URL in Safari and use **Share → Add to Home Screen**. The app stores its roster and game data in that browser on that device. It does not yet sync data between your phone and the coaches' devices; use Share or CSV export to send reports.

## Notes

- `index.html`, `app.js`, `manifest.webmanifest`, `sw.js`, and `icon.svg` are the app. No build step or server database is required.
- Events and roster are currently stored locally in the browser. Clear browser website data and the local records may be lost, so export CSV backups regularly.
- This is a working prototype, not an App Store-distributed product. It does not yet support a shared team account, cloud sync, multiple scorers, player photos, or permission-based coach access.
- PDF export opens the device's print flow. Choose its Save as PDF option where available.
