# Venstre / Højre

A single page that calls out random Danish directions in 60-second rounds:
"venstre … tilbage", "højre … tilbage", with random pauses in between.

Open `index.html` in a browser and press **Start**. A spoken 3-2-1 countdown
("tre, to, en") runs before each round. Speech uses the browser's
built-in text-to-speech with a Danish (`da-DK`) voice. If the device has no
Danish voice installed, the page shows a warning.

Use the **Tempo** slider (0.5×–2×) to shorten or lengthen the pauses. The
voice always speaks at normal speed. The setting is remembered in the browser.

Base timing at 1.0× (edit the constants at the top of the script to tune):
- direction → "tilbage": 0.35–1.0 s
- "tilbage" → next direction: 0.5–1.4 s

For a quick test, set the round length in the URL, e.g. `?seconds=10`:
https://madsandreasen.github.io/left-right/?seconds=10

## Install as an app

The page is a PWA (manifest + service worker), so it can be installed and works
offline:
- **Android / Chrome:** menu → *Install app* (or *Add to Home screen*).
- **iPhone / Safari:** Share → *Add to Home Screen*.

The service worker fetches the newest version whenever online and falls back to
the cached copy offline.
