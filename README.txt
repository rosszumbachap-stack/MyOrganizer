MyOrganizer PWA

Files:
- index.html
- manifest.webmanifest
- service-worker.js
- icon-192.png
- icon-512.png

IMPORTANT:
A PWA must be served over HTTPS or localhost. Opening index.html directly as a file will not allow
the service worker/installable PWA features to work.

Easy test on a computer:
1. Open a terminal in this folder.
2. Run:
   python -m http.server 8000
3. Open http://localhost:8000 in Chrome.

For Android installation:
Host this folder on any HTTPS web host (GitHub Pages, Netlify, Cloudflare Pages, etc.).
Then open the HTTPS URL in Chrome on Android and choose "Install app" or "Add to Home screen".

Your organizer content is stored locally in the browser on the device.
