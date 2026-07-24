# BMH Media Player

Static livestream overlay media player. The main overlay stays transparent and only appears while command media is playing.

## GitHub Pages

Publish this repository with GitHub Pages from the `main` branch root. The overlay URL will be:

```text
https://bigmervhuge.github.io/bmh-media-player/
```

## URL options

Use query options to tune the display without editing files:

```text
https://bigmervhuge.github.io/bmh-media-player/?scale=1&width=360&height=132
```

- `scale=1.2` makes command media larger. Try `0.8` to make it smaller.
- `width=420&height=160` sets the default media box size.

## Stream use

Add the GitHub Pages URL as a browser/web overlay if the mobile streaming app supports it. If it only supports pasted text or alerts, use this page from a remote browser source through desktop OBS as a fallback.

The overlay loads `styles.css` and `app.js` through `version.json`, then checks that file about once per minute. To force connected overlays to refresh after a code/style change, update the `version` value in `version.json` and push it with the change.

## Caldwell quotes

The current Version 3 quote list is mirrored in `data/caldwell-quotes.json`. The live overlay receives these through the Apps Script command endpoint.

## Video commands

Hosted command video assets are listed in `data/video-commands.json`.

- `!yeah` -> `assets/video/yeah.mp4`
- `!vb` -> `assets/video/vb.mp4`
- `!vamp` -> `assets/video/vamp.mp4`
- `!eels` -> `assets/video/eels.mp4`
- `!hoes` -> `assets/video/hoes.mp4`

Command URLs can also pass per-clip sizing to the Apps Script endpoint, such as `&width=420&height=160` or `&scale=1.25`.
