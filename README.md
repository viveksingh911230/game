# 🎮 Pixel Hopper — 2D & 3D Platformer

Two browser platformer games built with plain HTML5 + JavaScript. No build step, no install: each game is a single `index.html` file you can open in any modern browser.

| Game | Folder | Tech |
|------|--------|------|
| **Pixel Hopper (2D)** | [`pixel-hopper-2d/`](pixel-hopper-2d/index.html) | HTML5 Canvas, Web Audio |
| **Pixel Hopper 3D** | [`pixel-hopper-3d/`](pixel-hopper-3d/index.html) | Three.js (r128, via CDN), WebGL, Web Audio |

---

## ▶️ How to play

1. Download or clone this repo.
2. Open `pixel-hopper-2d/index.html` or `pixel-hopper-3d/index.html` in Chrome / Edge / Firefox.
3. Press **Space** (or tap) to start.

> The 3D game loads Three.js from `cdnjs.cloudflare.com`, so it needs an internet connection the first time it opens.

**Play online with GitHub Pages:** go to *Settings → Pages*, set *Source* to *Deploy from a branch*, pick `main` / root, and save. Then the games are at
`https://<your-username>.github.io/<repo-name>/pixel-hopper-2d/` and `.../pixel-hopper-3d/`.

---

## 🕹️ Controls

### 2D
| Action | Keys |
|---|---|
| Move | ← → or A / D |
| Jump (hold for higher) | Space, ↑, W or Z |
| Pause | P |
| Mobile | On-screen ◀ ▶ ▲ buttons |

### 3D
| Action | Keys |
|---|---|
| Run along the course | ← → or A / D |
| Move in depth | ↑ ↓ or W / S |
| Jump (hold for higher) | Space, Z or J |
| Switch camera (Side / Chase) | C |
| Pause | P |
| Mobile | 4-way pad + jump + CAM buttons |

In **Chase** camera, ↑ runs forward and ← → strafe.

---

## 🌍 Levels

1. **Green Hills**: grassy intro with gentle gaps and the first enemies
2. **Sky Steps**: sunset world with spike pits and one-way platforms
3. **Ember Keep**: dark castle with stone towers, tight jumps and more enemies

## ✨ Features

- Run, jump and stomp enemies; avoid spikes and pits
- Coins, score, lives (3) and a level timer with a time bonus at each flag
- Smooth controls: coyote time, jump buffering, variable jump height
- Particle effects and retro sound effects made with the Web Audio API
- Fixed 60 Hz physics step, so it plays the same on any refresh rate
- Touch controls on phones and tablets
- **3D only:** voxel levels with real-time shadows, a blob shadow under the player to judge landings, two camera modes, falling off platform edges, animated blocky hero

## 🛠️ Editing levels

Levels are text maps at the top of each file (`const LEVELS = [...]`). Both games use the same map format:

| Char | Meaning |
|---|---|
| `#` | Ground |
| `=` | Brick block |
| `-` | One-way platform (jump up through it) |
| `^` | Spikes |
| `o` | Coin |
| `E` | Enemy |
| `P` | Player start |
| `F` | Goal flag |

Change a map in one game and copy it into the other to keep both versions in sync.

## 📦 Publishing on itch.io

Zip either game folder (with `index.html` at the top level), upload it as an **HTML** project and tick *"This file will be played in the browser"*.

---

Made by **Vivek Kumar Singh** · Genius Bro!
