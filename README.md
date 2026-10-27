# ONHS Online Express — Oleras National High School

A responsive, installable static website/PWA prototype with News, Feature, Editorial (including editorial cartoon), Sports, Literary, Announcements, Trivia ticker, About Us, and a browser-based admin CMS.

## Run locally

Because the site uses a service worker, run it through a local web server rather than opening `index.html` directly. With Python installed, open a terminal in this folder and run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`. Open `admin.html` to manage content.

## CMS capabilities

- Add, edit, publish/unpublish, and delete stories by section.
- Edit announcements and their full details.
- Replace the upper banner image and editorial cartoon image by URL or upload.
- Edit tagline, About Us text, cartoon title/message, and scrolling trivia.
- Export and import JSON backups.
- Uploaded images are stored as browser data URLs; for this demo, choose images smaller than 1.5 MB.

## Important limitations

This is a functional front-end prototype. CMS edits are stored in `localStorage` in the current browser only; they are not shared with other visitors/devices and may be cleared with browser data. A public production deployment needs a backend/database, secure administrator authentication, shared media storage, and hosting. Google Fonts and sample Unsplash photos require an internet connection. Replace all sample copy and imagery with approved school content before publishing.

## Brand assets

The supplied ONHS Online Express logo is in `assets/online-express-logo.png`. A copy of the supplied website mockup reference is in `assets/website-mockup-reference.png`.
