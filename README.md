# Business Trip Tracker

A simple PWA for tracking business trips for tax purposes. Record start/end times of your trips, export logs as CSV, and back up your data — all from your phone.

## Features

- **Start/Stop trips** — tap to record departure and return with exact timestamps
- **Add past trips manually** — forgot to start one? Add it retroactively with date/time pickers
- **CSV export** — download your trip log with city, country, dates, times, and number of days
- **Backup & restore** — export/import your data as JSON so nothing gets lost
- **Works offline** — service worker caches the app for offline use
- **Install on phone** — add to home screen via Safari (iOS) or Chrome (Android) for a native app feel

## Setup

No build step required. Serve the files with any static file server:

```sh
# using python
python3 -m http.server 8000

# or using npx
npx serve .
```

Then open `http://localhost:8000` in your browser.

## Hosting

Deploy to any static hosting provider:

- **GitHub Pages** — push to GitHub and enable Pages in repo settings
- **Netlify** — drag and drop the folder or connect your repo
- **Vercel** — import the repo and deploy

HTTPS is required for the PWA service worker to function on mobile.

## Data Storage

All data is stored locally in the browser via `localStorage`. Use the **Backup Data** button to export a JSON file you can save to iCloud, Google Drive, or any cloud storage for safekeeping.
