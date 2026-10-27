# Online EXPRESS — Website/PWA prototype

A responsive static website prototype for Oleras National High School's Online EXPRESS publication.

## Files
- `index.html` — website layout and styling
- `app.js` — sample stories, navigation, article views, and browser-local admin CMS
- `logo.png` — your supplied Online EXPRESS logo
- `manifest.webmanifest` — PWA metadata
- `service-worker.js` — basic offline caching for the app shell

## Run locally
For a quick preview, open `index.html` in a modern browser. PWA installation and service-worker offline caching require a local web server or HTTPS.

If Python is installed, open a terminal in this folder and run:
`python -m http.server 8000`
Then visit `http://localhost:8000`.

## Admin CMS
Choose **ADMIN CMS** in the navigation. You can add, edit, publish/draft, or delete articles and cartoon editorials. Data is stored in that browser's `localStorage`, so it is only a prototype:
- content is not shared across devices or staff accounts
- clearing browser data may erase edits
- no administrator authentication or server-side database is included

## Before official deployment
1. Replace all placeholder stories, dates, images, and captions with verified school content.
2. Use an original approved school publication logo if required.
3. Add secure admin login, server/database storage, image uploads, backup, and moderation workflow.
4. Serve through HTTPS and review privacy, child-protection, consent, and publication policies.
5. Google Fonts and sample images load from external services; provide locally hosted assets if full offline use is required.

No payments or payment forms are included.
