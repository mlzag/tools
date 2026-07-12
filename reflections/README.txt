EVENING REFLECTION — APP PACKAGE
==================================

This folder is a tiny installable web app:

  index.html
  manifest.json
  icons/
    favicon.ico
    icon-16.png, icon-32.png, icon-152.png, icon-180.png,
    icon-192.png, icon-512.png, icon-master.png

Keep these files together in this same folder structure — index.html
looks for manifest.json and icons/ right next to it.

HOW TO GET THE CRESCENT-MOON ICON ON YOUR HOME SCREEN
-------------------------------------------------------

Custom icons on a phone home screen require the page to be loaded
over http/https (not opened directly as a local file). Two easy ways:

OPTION A — Free static hosting (2 minutes, most reliable)
  1. Go to https://app.netlify.com/drop on a computer.
  2. Drag this whole folder onto the page. It gives you a live URL.
  3. Open that URL on your phone.
     - iPhone (Safari): tap Share → "Add to Home Screen"
     - Android (Chrome): tap the ⋮ menu → "Install app" (or you'll
       see an automatic install banner)
  4. The moon icon will be used automatically.

OPTION B — Run it locally on your own Wi-Fi
  1. On a computer, open a terminal in this folder and run:
       python3 -m http.server 8000
  2. Find your computer's local IP address (e.g. 192.168.1.23).
  3. On your phone, open http://192.168.1.23:8000 in the browser
     (must be on the same Wi-Fi network).
  4. Add to Home Screen as above.

WITHOUT HOSTING
  You can still just open index.html directly on your phone (e.g.
  via AirDrop, email, or a files app) — the reflection tool works
  exactly the same. You just won't get the custom moon icon; it'll
  use your browser's default bookmark icon instead.

Your entries are stored locally in the browser/app you open it in,
and — if you connect a folder in Settings — mirrored to a
reflections.md or reflections.json file on your device.
