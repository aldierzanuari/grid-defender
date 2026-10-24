# GRID DEFENDER: BLACKOUT SIEGE — playable expo prototype

Game portrait HTML5 Canvas, no server required, hosted by GitHub Pages.

## Installation
Upload **index.html**, **game.js**, and the **assets** folder to the root of the `grid-defender` repository (keep folder paths). Pages should publish from `main / (root)`.

## Controls
Tap enemies to shoot; EMP stuns and damages; Turret Drone auto-attacks for 10 seconds; Overcharge clears enemies when 100%. Pause button. 105-second survival. Local top scores via localStorage.

## Integration with existing Apps Script Energy Play Arena
The existing `Games.html` dynamically loads only `smartgrid` and `voltrush` through `getGamePage()`. For a third card, easiest is an external link to this GitHub Pages URL (rather than passing this game through GAS). See `GAS_INTEGRATION.txt` for an optional snippet.

## Visual limitations
This is a **playable cinematic 2.5D prototype** using the supplied concept artwork as a background. Enemies are procedurally drawn Canvas graphics; these are **not photorealistic GLB models**. The reference concept contains baked-in HUD, enemies, and weapon, which can appear beneath live elements. For production, replace it with a clean background plate and authored transparent enemy/weapon sprites or rigged 3D models. The concept art is not a functional 3D asset.

## Score storage
Scores are **per-browser only**, not shared across devices. A cross-device leaderboard requires a separate backend such as Apps Script + Sheets with abuse protection.

## Performance
Optimized for portrait, including mouse and touch. Requires modern browser; audio begins after user interaction. All assets served from GitHub Pages.
