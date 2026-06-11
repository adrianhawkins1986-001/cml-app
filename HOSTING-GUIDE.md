# CML Field App — putting it on your iPad

The app lives in this folder (index.html + manifest.json + sw.js + icons). To make it an installable iPad app, host the folder for free on GitHub Pages, then add it to the iPad home screen.

## One-time setup (10 minutes, on any computer)

1. Create a free account at https://github.com (skip if you have one).
2. Click the "+" (top right) → "New repository". Name it `cml-app`, set it to **Public**, tick "Add a README", click "Create repository".
3. In the new repository, click "Add file" → "Upload files". Drag in ALL the files from this `cml-field-app` folder (index.html, manifest.json, sw.js, and the three icon PNGs). Click "Commit changes".
4. Go to Settings → Pages (left sidebar). Under "Branch", choose `main` and `/ (root)`, click Save.
5. After a minute or two, the page shows your app's address, e.g. `https://YOURNAME.github.io/cml-app/`

## On the iPad (once per device)

1. Open Safari and go to that address.
2. Tap the Share icon → **Add to Home Screen** → Add.
3. The CML icon appears on the home screen. It opens full-screen like a normal app and keeps working offline after the first load.

## Day-to-day use

- Each pipework keeps its own CML register and readings — switch with the PIPEWORK dropdown.
- Everything autosaves to the device as you type ("SAVED" indicator in the bar).
- **Back up regularly**: tap BACKUP to download a .json file of all pipeworks. RESTORE loads it back — on the same iPad or a different device.
- Data is stored per device. To move work between devices, use BACKUP/RESTORE or the Excel export.

## Updating the app later

Upload the changed file(s) to the GitHub repository the same way (Add file → Upload files — it overwrites). After updating, bump the cache name in sw.js (e.g. `cml-field-app-v2`) so iPads pick up the new version on next launch. Your stored readings are NOT affected by app updates.
