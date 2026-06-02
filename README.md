# Seeking the Deep

Turn-based underwater rogue-lite in vanilla JavaScript (PWA).

## Description

Explore procedurally generated ocean depths, fight deep-sea creatures, and collect pearls. Oxygen is limited — every action brings you closer to death. Collected pearls persist between runs and can be used to purchase permanent upgrades.

## Features

- Procedural map generation (cellular automaton, 4 smoothing iterations)
- BFS-based fog of war (unexplored / explored / visible)
- 4 enemy types with different behavior (patrol / chase)
- 5 item types (Pearl, O₂ Tank, Medkit, Harpoon, Glow Stone)
- Meta-progression: permanent upgrade shop using pearls
- Mobile controls (on-screen D-pad)
- PWA: works offline, installable on device

## Running

Open `seeking-the-deep.html` in a browser, or serve the directory via any HTTP server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/seeking-the-deep.html

## Files

| File | Purpose |
|---|---|
| `seeking-the-deep.html` | Game |
| `game-mechanics.html` | Mechanics documentation (map generation, visibility) |
| `sw.js` | Service Worker (PWA, offline cache) |
| `manifest.json` | Web App Manifest |
| `icon-192.png` / `icon-512.png` | PWA icons |

## License

MIT
