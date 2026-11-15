# Community Bridge

A free, multilingual, voice-enabled community-resource finder for Fellsmere, Sebastian, and Vero Beach, Florida — built for people who may not type or read comfortably.

**Live demo:** https://mrjosueayalaperez-dev.github.io/Community-Bridge-/

## What it does

- **Four languages:** English, Spanish, Haitian Creole (Kreyòl), and Portuguese — full interface and listings in each.
- **Voice and text:** ask by microphone (browser speech recognition) or type; listings can be read aloud (browser speech synthesis). Every voice feature has a silent typed equivalent.
- **Categories:** crisis lines, food, housing, health, mental health, jobs, legal help, transportation, childcare, utilities, seniors, mobility equipment, and education.
- **Local + national:** verified local listings for the Fellsmere–Sebastian–Vero Beach area, plus national lines (211, 988, USDA Hunger Hotline). Each local listing shows its source and the date it was verified; users are advised to confirm hours and eligibility before traveling.
- **A recorded greeting** from the Professor (the platform's teacher figure) in all four languages, with captions.
- **No account, no cost, no tracking:** it is a single static page. Typed searches are processed in the visitor's browser and sent nowhere.

## How it works

- One self-contained `index.html` (HTML, CSS, and JavaScript in a single file) — no backend, no database, no build step.
- Listings and translations live in data tables inside the file; the question router is keyword-based (it is a directory search, not an AI).
- Served by GitHub Pages from the `main` branch of this repository.

## Repository contents

- `index.html` — the application
- `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` — Progressive Web App support (installable, offline shell)
- `logo-community-bridge.jpg` — the Community Bridge logo artwork (source for the app icons and favicons)
- `professor-greeting-cb-EN.mp4` / `-ES` / `-HT` / `-PT` — greeting videos
- `captions-en.vtt` / `-es` / `-ht` / `-pt` — caption tracks for the greeting
- `cb-professor.jpg` — Professor image / video poster

## Install it on a phone

Community Bridge is an installable Progressive Web App. On Android Chrome: open the live site, tap the ⋮ menu, then **Install app** (or **Add to Home screen**). On iPhone Safari: tap **Share**, then **Add to Home Screen**. No app store, no account, no cost. After the first visit, the app shell also opens with a weak or missing connection.

## Run it locally

Open `index.html` in any modern browser, or serve the folder with any static file server. Voice input requires Chrome or Edge (the web speech-recognition API); everything else works in any current browser.

## Ownership and license

Copyright (c) 2026 Josue Ayala-Perez. All rights reserved — see `LICENSE`. Community Bridge is a product of the M&Q Ecosystem.

## Contact

Community Bridge is a free community resource. For questions about a specific listing, please contact that organization directly — every listing shows its own phone number and address. Please confirm hours and eligibility before traveling.
