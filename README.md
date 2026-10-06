# Venstre / Højre

A single page that calls out random Danish directions in 60-second rounds:
"venstre … tilbage", "højre … tilbage", with random pauses in between.

Open `index.html` in a browser and press **Start**. Speech uses the browser's
built-in text-to-speech with a Danish (`da-DK`) voice. If the device has no
Danish voice installed, the page shows a warning.

Timing (edit the constants at the top of the script to tune):
- direction → "tilbage": 0.5–1.3 s
- "tilbage" → next direction: 0.7–1.8 s
