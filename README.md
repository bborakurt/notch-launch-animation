# Notch Launch Animation

A first-launch animation that opens out of a laptop notch: the notch floods open and bursts into coloured dust, a pair of eyes forms and says hello, the dust is reeled into progress rings, and the island folds back into a bar.

**One file, `index.html`.** Plain SVG and JavaScript: no libraries, no build step, no assets. Open it in a browser.

## Make it yours

Everything is in that one file, top to bottom:

1. **SETTINGS**: colours, rings (any number), text, sizes, speed and timing, and which effect plays each phase.
2. **CORE**: stage, rings, dust, clock and playback. Its header explains how to write an effect.
3. **EFFECTS**: the animation's four phases, each one swappable:
   - `opening`: how the island opens and where the dust hangs
   - `character`: the eyes (or `"none"`)
   - `fill`: how the dust travels into the rings, and how the rings fill
   - `closing`: how the island closes and what stays on screen

Small changes are a line in SETTINGS. For a different motion, write a new effect for that phase and select it; the rest keeps working.

**With an AI assistant:** give it the whole file and describe what you want, e.g. *"make the dust spiral into the rings"*, *"replace the eyes with a smiling face"*, *"make the rings fill in steps"*. Everything it needs is in the file.

In the browser console, `notchLaunch.seek(3.5)` jumps to 3.5 s and `notchLaunch.play()` replays.

## Licence

MIT. See `LICENSE`.
