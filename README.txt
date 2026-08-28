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


VERSION 2 UPDATE
----------------
Settings now includes Backup & Restore.

Export Backup:
- Settings > Backup & Restore > EXPORT BACKUP
- Save the JSON file to Google Drive, Files, or another safe location.

Restore:
- Install/open MyOrganizer on the new device.
- Settings > Backup & Restore > IMPORT BACKUP
- Select the previously exported JSON file.
- Confirm restore.

The backup includes:
- Calendar events
- Shopping items
- Financial entries
- General notes
- Goals

GitHub Pages update:
Upload the updated index.html and service-worker.js to your existing repository.
The service worker cache version has been bumped to v2 so installed PWAs can refresh.
