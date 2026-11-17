# jamesmullally.com

Personal homepage: stand on a shale beach, look across a lake, and flick a stone to skip it.

- `index.html` is the whole page: one canvas scene plus a few corner labels. No build step.
- The scene follows the visitor's local clock (sunrise, day, sunset, night).
- A harder flick gives more skips, from 2-3 up to about 15. The buoy is solid.
- `sounds/` holds the two public-domain recordings the page plays. Sources are in `sounds/CREDITS.txt`.

## Running it

Serve the folder with any static server, for example:

```bash
python -m http.server 8091
```

Opening `index.html` straight from disk shows the scene but not the sound, because browsers block loading the audio files from a `file://` page.

## Not done yet

- `index.html` has no `<!doctype html>`, `<html>` or `<body>` wrapper, because it is also published as a Claude artifact, which adds its own. Add the wrapper before deploying it to the real domain.
- Not yet deployed; jamesmullally.com still redirects to LinkedIn.
