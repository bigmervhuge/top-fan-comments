# BMH Media Player

Static livestream overlay media player.

## GitHub Pages

Publish this repository with GitHub Pages from the `main` branch root. The overlay URL will be:

```text
https://bigmervhuge.github.io/bmh-media-player/
```

## URL options

Use query options to tune the display without editing files:

```text
https://bigmervhuge.github.io/bmh-media-player/?seconds=9&scale=1
```

- `seconds=9` changes how long each comment stays on screen.
- `scale=1.2` makes the overlay larger. Try `0.8` to make it smaller.
- Default display is a compact top-left box.
- `position=bottom`, `top`, `middle`, `left`, or `right` expands it to a full overlay canvas and moves the box.
- `meta=0` hides the username/timestamp line.
- `clean=1` removes the dark box and leaves only text shadow.
- `paused=1` stops auto-rotation. Tap/click, Space, Enter, or the right arrow advances manually.
- `random=0` turns off the default random order.
- `user=TheLetterM` or `user=OlTrouty` filters to one user.

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
