# Draw Wheal — Draw. Roll. Conquer.

**Draw a wheel. Mount it. Drive your way through five themed levels.**

Draw Wheal is a responsive, vanilla HTML5 Canvas game. Use your mouse or touch to sketch a tyre, then drive the little red buggy over rolling terrain, collect coins, jump over bumps, and unlock new tracks.

## Play locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Press **Play**, draw your wheel, mount it, and drive.

No build step or framework installation is required. The game has a keyboard and touch-friendly control layout.

## Controls

- **D / →** — accelerate
- **A / ←** — brake / reverse
- **Space / ↑ / W** — jump
- **P** — pause / resume
- **Draw Wheel** — open the sketch pad and replace your tyre shape
- On mobile, use the on-screen arrows and jump control.

## Game features

- Five levels with different visual themes: Sunny Hills, Dusty Dunes, Pinewood Pass, Frostbite Ridge, and Neon Night Run.
- Mouse/touch wheel drawing with sketch normalization.
- Rolling terrain, camera follow, jumps, coins, a finish gate, level unlocks, and pause/restart controls.
- Progress-based level unlocking saved locally in the browser.
- Responsive canvas layout; no game-engine dependency.

## Asset library

All art is stored as **individual SVG files**, not as a composite collage or approximate sprite-sheet crops.

- `assets/frames/idle/` — 10 complete idle/suspension frames
- `assets/frames/drive/` — 12 complete driving/rolling frames
- `assets/frames/jump/` — 10 complete jump frames
- `assets/frames/fall/` — 10 complete falling/landing frames
- `assets/frames/crash/` — 10 complete impact/skid frames
- `assets/backgrounds/` — five separate level backgrounds
- `assets/wheels/` — round, chunky, neon, and snow wheel designs
- `assets/textures/` — rock, desert, forest, and snow ground tiles
- `assets/ui/` — coin, finish flag, star, and button artwork
- `assets/cars/` — car body and complete red car reference art

The 52 car animation frames use the same 512 × 300 canvas and transparent background, and each file contains the complete car. The game itself draws the player wheel from the live sketch so the selected shape remains changeable during play.

## Publish with GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. Open the Pages URL shown on that settings page.

The game uses the open-source **Nunito** web font when online; Trebuchet MS and system UI are fallbacks. For fully offline font delivery, add a properly licensed WOFF2 file in `assets/fonts/` and wire it through `@font-face`.

## Project structure

```
index.html
assets/
  backgrounds/
  cars/
  fonts/
  frames/
    idle/
    drive/
    jump/
    fall/
    crash/
  textures/
  ui/
  wheels/
```
