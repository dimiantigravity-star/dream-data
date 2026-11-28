# dream-data

Data packs for the Dream launcher's Online tab. Not hand-edited: built by `node scripts/parse-doodle.mjs` in the Dream project.

- `manifest.json`: `v` goes up every time the pack changes; the app downloads the files only when its stored copy is older or after an app update.
- `doodle-games.json`: `[{slug, name, id}]`, the game list (`id` = the public embed page of each game).
- `doodle-covers.json`: `{slug: base64 WebP 144x144}`.
- `featured/`: full-size art used by the app's update reel.
- `html/<slug>.html`: each game's own page (the HTML inside its Apps Script embed). The app runs it with the ads switched off and loads one only when that game is opened; the Apps Script page stays the fallback.
