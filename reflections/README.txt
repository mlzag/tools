EVENING REFLECTION — APP PACKAGE
==================================

A quiet, five-step wind-down ritual: reflect on your day, then refocus
on your priorities before bed.

FOLDER CONTENTS
----------------
  index.html
  manifest.json
  icons/
    favicon.ico
    icon-16.png, icon-32.png, icon-152.png, icon-180.png,
    icon-192.png, icon-512.png, icon-master.png

Keep these files together in this same folder structure — index.html
looks for manifest.json and icons/ right next to it.

FEATURES
---------
- Five-step flow: highlight, stressor/growth, priorities, non-negotiables,
  close-out — each with rotating prompt variations
- Swipe left/right (or tap the arrow icons) to move between steps
- Minimal sticky footer nav with step dots — never overlaps content,
  and the middle of the screen scrolls independently if a step runs long
- Date shown persistently in the header
- Settings menu (gear icon): rename or add/remove priorities and
  non-negotiables, choose export format, connect a folder to save to
- Entries save automatically per day, locally in the browser
- Optional folder sync to a single reflections.md or reflections.json
  file (Chrome/Edge only — see below)
- Installable as a home-screen app with a custom crescent-moon icon

HOW TO GET THE CRESCENT-MOON ICON ON YOUR HOME SCREEN
-------------------------------------------------------
Custom icons on a phone home screen require the page to be loaded
over http/https (not opened directly as a local file).

If you're hosting on GitHub Pages:
  1. Push this folder's contents to your repo (see below).
  2. Enable Pages under Settings → Pages, and note the live URL
     GitHub gives you (it will look like
     https://yourusername.github.io/reponame/).
  3. Open that URL on your phone.
     - iPhone (Safari): tap Share → "Add to Home Screen"
     - Android (Chrome): tap the ⋮ menu → "Install app"
  4. The moon icon is picked up automatically from manifest.json.

WITHOUT HOSTING
  You can still open index.html directly on your phone — the tool
  works the same. You just won't get the custom moon icon; it'll use
  your browser's default bookmark icon instead.

FOLDER-SYNC STORAGE NOTE
--------------------------
The "Choose folder" option in Settings uses the File System Access
API, which currently only works in Chromium browsers (Chrome, Edge)
and needs to be reconnected each session — it isn't persisted across
page reloads. Your entries are always saved locally regardless, and
you can use "Export now" in Settings anytime to download a copy.

PUSHING UPDATES TO YOUR REPO
------------------------------
From inside this folder:
  git add index.html manifest.json README.txt icons
  git commit -m "Update reflection app UI"
  git push

GitHub Pages will redeploy automatically within a minute or two —
no need to redo "Add to Home Screen" afterward.
