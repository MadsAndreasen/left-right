# Venstre / Højre

A single page that calls out random Danish directions in 60-second rounds:
"venstre … tilbage", "højre … tilbage", with random pauses in between.

Open `index.html` in a browser and press **Start**. Speech uses the browser's
built-in text-to-speech with a Danish (`da-DK`) voice. If the device has no
Danish voice installed, the page shows a warning.

Timing (edit the constants at the top of the script to tune):
- direction → "tilbage": 0.25–0.7 s
- "tilbage" → next direction: 0.35–1.0 s

For a quick test, set the round length in the URL, e.g. `?seconds=10`:
https://madsandreasen.github.io/left-right/?seconds=10
