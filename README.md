# Instructor Hub

Offline flight-instructor tool (iPad, phone, desktop):

- **Today** – the day's plan by student. Each item carries a preflight section (airport, runway, winds,
  altimeter, ATIS, squawk, fuel/oil, HOBBS, times, METAR/TAF, NOTAM), the pre-flight briefing
  (PGI, objectives, threats & errors) and the post-flight debrief (what went well, areas for
  remediation, study assigned, plan for next lesson). Print a day sheet or an item; email a debrief.
- **Students** – student list, open/resolved areas for remediation, upcoming items, history and flight tests.
- **Flight Test** – marking sheets for the RPP, PPL and CPL flight tests laid out like the TC flight test
  reports. Each exercise shows the Performance Criteria from the Flight Test Guide as pills; tap once for
  a minor, twice for a major, three times for a critical deviation. The app suggests the mark (weakest
  element) and works out pass/fail, partial or complete re-test. Print the report, email it, or send the
  major/critical deviations to the student's remediation list.
- **Settings** – instructor name, aircraft, Preflight Briefing link, sync and backup.

## Sync
Data lives on each device and is synced through a **secret GitHub Gist** in your account
(`instructor-hub.json`). On each device: Settings → paste a fine-grained personal access token with
**Account permissions → Gists: Read and write**. The app finds or creates the gist itself.

## Files
- `index.html` – the app
- `ftg-data.js` – Performance Criteria from the Flight Test Guides (RPP TP 12475E, PPL TP 13723E, CPL TP 13462E)
- `sw.js` – offline cache. Change `VERSION` whenever you upload new files.
- `manifest.webmanifest`, icons – home-screen install

## GitHub Pages
Settings → Pages → Deploy from branch → `main` / root. Open
`https://macord-tech.github.io/instructor-tools/` once while online, then Share → Add to Home Screen.

Training aid only. The Flight Test Guides and the examiner's assessment govern.
