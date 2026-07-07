# Beach Buggy Racer 🏖️

**▶ Play it:** https://github.freaxnx01.ch/game-beach-buggy-racer/

A single-file isometric arcade racer: dirt track on a tropical beach with tabletop jumps, whoops, berms, a water ford, and boost pads. Inspired by the look of top-down/iso racers like Super Woden GP.

**Play:** open `index.html` in any browser — no build, no dependencies (one Google Fonts link; degrades gracefully offline).

## Controls
- **Space / ↑ / W** — accelerate
- **← → / A D** — steer
- **↓ / S** — brake / reverse
- **Ctrl** — handbrake drift
- **R** — reset car · **M** — mute

## Features
- Fixed isometric camera with speed-based zoom and look-ahead
- Physics: airtime off jumps, whoops chatter, surface grip (dirt / sand / water)
- Lap timing with best-lap persistence (localStorage)
- Synthesized audio (Web Audio): engine, skids, boost, splash, lap chime — no audio files
- Skid marks, dust, splash particles; palm trees, umbrellas, tire stacks

## Tech
Pure HTML + Canvas 2D + vanilla JS in one file. Track is a Catmull-Rom spline; ground is pre-rendered to an offscreen canvas; sprites are depth-sorted each frame. Fixed-timestep physics at 120 Hz.