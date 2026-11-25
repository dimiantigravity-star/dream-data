# dream-data

Data packs for the Dream launcher's Online tab. Not hand-edited: built by `node scripts/parse-doodle.mjs` in the Dream project.

- `manifest.json`: `v` goes up every time the pack changes; the app downloads the files only when its stored copy is older or after an app update.
- `doodle-games.json`: `[{slug, name, id}]`, the game list (`id` = the public embed page of each game).
- `doodle-covers.json`: `{slug: base64 WebP 144x144}`.
