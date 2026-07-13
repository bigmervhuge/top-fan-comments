# Top Fan Comments

Static livestream overlay for rotating curated comments one at a time.

## GitHub Pages

Publish this repository with GitHub Pages from the `main` branch root. The overlay URL will be:

```text
https://bigmervhuge.github.io/top-fan-comments/
```

## URL options

Use query options to tune the display without editing files:

```text
https://bigmervhuge.github.io/top-fan-comments/?seconds=9&scale=1&position=bottom
```

- `seconds=9` changes how long each comment stays on screen.
- `scale=1.2` makes the overlay larger. Try `0.8` to make it smaller.
- `position=bottom`, `top`, `middle`, `left`, or `right` moves it.
- `meta=0` hides the username/channel/timestamp line.
- `count=0` hides the comment counter.
- `clean=1` removes the dark box and leaves only text shadow.
- `paused=1` stops auto-rotation. Tap/click, Space, Enter, or the right arrow advances manually.
- `user=TheLetterM` or `user=OlTrouty` filters to one user.

## Stream use

Add the GitHub Pages URL as a browser/web overlay if the mobile streaming app supports it. If it only supports pasted text or alerts, use this page from a remote browser source through desktop OBS as a fallback.
