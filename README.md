# ironlog
# IronLog — Workout Tracker

A lightweight, offline-first Progressive Web App for tracking gym workouts. Log exercises, monitor personal records, and review your training history — no account required, no data leaves your device.
---
## Live App

[Open IronLog](https://YOUR-USERNAME.github.io/ironlog/)

> Replace `YOUR-USERNAME` with your actual GitHub username.

---

## Install on Your Phone
**Android (Chrome)**
1. Open the link above in Chrome
2. Tap the "Add to Home Screen" banner at the bottom
3. If the banner doesn't appear, tap the three-dot menu and select "Add to Home Screen"
4. The app icon will appear on your home screen

**iPhone (Safari)**
1. Open the link in Safari
2. Tap the Share button at the bottom
3. Select "Add to Home Screen" and tap Add

---
## Features

**LOG**
- Record exercises with muscle group, name, equipment, weight, sets, reps, and notes
- Autocomplete suggestions based on the selected muscle group
- Edit or delete any entry on the current day
- Quick stats per session: total exercises, muscles worked, max weight, total volume

**HISTORY**
- Browse all past workout days, newest first
- Edit any past exercise inline without switching tabs
- Delete entries with a confirmation step

**STATS**
- Summary of total days trained, exercises logged, and daily average
- Muscle group breakdown showing which areas you train most
- Monthly volume chart to track total tonnage over time
- Personal records per exercise with full weight history

**General**
- Works offline after the first load
- Data is stored locally on your device — nothing is sent anywhere
- Installable as a standalone app on Android and iOS
- Responsive layout built for mobile use

---

## File Structure

```
ironlog/
├── index.html       — Full app: markup, styles, and logic in one file
├── manifest.json    — PWA config: name, icons, display settings
├── sw.js            — Service worker for offline caching
├── icon-192.png     — App icon for home screen
└── icon-512.png     — App icon for splash screen
```

---
## Tech Stack

| Layer       | Details                                 |
|-------------|-----------------------------------------|
| Frontend    | Vanilla HTML, CSS, JavaScript           |
| Fonts       | Barlow Condensed, Barlow (Google Fonts) |
| Storage     | localStorage (on-device)                |
| Offline     | Service Worker with Cache API           |
| Installable | Web App Manifest                        |

No frameworks, no build tools, no dependencies. The entire app is a single HTML file.

---
## Running Locally

```bash
git clone https://github.com/YOUR-USERNAME/ironlog.git
cd ironlog

# Simple — open directly in browser (Service Worker won't register over file://)
open index.html

# Full PWA — serve over localhost
npx serve .
# Then visit http://localhost:3000
```

---

## Privacy

All workout data is stored in your browser's localStorage. Nothing is sent to any server. There are no accounts, no analytics, and no third-party tracking. The only external request is loading fonts from Google Fonts on the first visit.

---

## License

MIT — free to use, modify, and distribute.
