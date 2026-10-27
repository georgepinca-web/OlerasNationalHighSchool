# Online EXPRESS — Oleras National High School

A responsive school publication website and installable PWA prototype using the supplied publication logo and blue/yellow branding.

## Included files
- `index.html` — responsive layout, Home, News, Editorial, Announcements, About Us, and Admin CMS views
- `app.js` — sample content, navigation, full article view, editable content manager, local image handling, and editable About Us details
- `logo.png` — supplied Online EXPRESS logo
- `manifest.webmanifest` — PWA metadata
- `service-worker.js` — basic app-shell caching for offline access after first load

## Preview locally
You can open `index.html` directly for a basic preview. To test PWA installation and offline caching, run a local web server from this folder:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` in your browser. PWA installation requires HTTPS or localhost.

## Edit content with Admin CMS
1. Open the site and choose **ADMIN CMS**.
2. Use **Articles** to edit or delete existing news, editorials, and announcements.
3. Use **Cartoons** to edit or delete cartoon editorials.
4. Use **Add Content** to add new content, select a publication type, add a story, author, date, photo caption, and image URL or upload an image file.
5. Use **About Us** to edit the publication description, tagline, and purpose.

Changes are saved in the current browser's local storage. Uploaded images are resized and stored in that browser. Content is not synchronized across computers or staff members.

## Important production notes
This is a no-payment, static prototype. It does not include administrator authentication, server-side storage, or shared multi-user editing. Before official public deployment, add secure admin sign-in, database storage, file hosting/backups, moderation, and a publication approval process. Replace all sample articles, dates, photos, captions, and cartoon messages with verified school content and approved images. Respect student privacy and obtain required consent before publishing identifiable learner photos.

Google Fonts and sample photos use external URLs; full offline use of all remote images/fonts is not guaranteed. The service worker caches the local app shell.
