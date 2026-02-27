# Coldwater Demo — Project Notes

## Project Type
Single-file browser games and demos. No framework, no build step, no server required. Everything ships as a standalone `.html` file openable directly in a browser.

## Stack
- Vanilla HTML/CSS/JS
- Canvas 2D API for game rendering
- Google Fonts via CDN (Press Start 2P, Orbitron)
- No npm, no bundler, no dependencies

## Files
- `carwash-simulator.html` — Arcade timing game. Car moves upward through a tunnel; player clicks color-coded buttons on tunnel walls to remove matching dirt spots from the car.

## Aesthetic
- Retro arcade / neon-on-dark
- Background: `#0a0a0f`, tunnel walls: `#1a1a2e`
- Neon accent colors: cyan `#00f5ff`, green `#39ff14`, pink `#ff0080`
- Fonts: Press Start 2P (headings), Orbitron (labels/HUD)

## Code Conventions
- Use `textContent` and safe DOM methods — never `innerHTML` with dynamic data
- Unicode escapes for special characters in JS strings (e.g. `\u2713` not `✓`)
- All game logic in a single `<script>` block at bottom of file
- CSS variables in `:root` for color palette
- `gameState` string drives screen visibility (`'title'`, `'playing'`, `'result'`)
