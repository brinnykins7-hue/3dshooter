# 🎯 ARENA FPS

A fast-paced browser-based first-person shooter built with Three.js. Inspired by the movement feel of Rivals and the weapon/UI systems of Counter-Strike 2.

![ARENA FPS](https://img.shields.io/badge/engine-Three.js%20r128-blue?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Web%20Browser-green?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-orange?style=flat-square)

---

## 🕹️ Controls

| Key | Action |
|-----|--------|
| `W A S D` | Move |
| `Space` | Jump |
| `Shift` | Slide (while sprinting) |
| `Ctrl` | Crouch |
| `Wall + Space` | Wall Jump |
| `LMB` | Shoot |
| `RMB` | ADS (Aim Down Sights) |
| `R` | Reload |
| `1` | Primary Weapon |
| `2` | Secondary / Pistol |
| `3` | Knife (fastest movement) |
| `B` | Open Weapon Buy Menu |
| `Esc` | Close Menu / Pause |

---

## ⚡ Movement System

### Sliding
Sprint and press `Shift` to trigger a momentum-based slide. You maintain your current velocity and glide at high speed. Sliding ends after ~0.6 seconds or when you leave the ground.

### Wall Jumping
Approach any wall while airborne and press `Space`. The game detects wall proximity in four cardinal directions and launches you off with a directional boost. Has a small cooldown to prevent infinite wall-riding.

### Speed Multipliers by Weapon
Equipping heavier weapons slows you down. Knife gives a speed bonus.

| Weapon Class | Speed |
|---|---|
| Knife | 115% |
| Pistol | 97–100% |
| SMG | 91–95% |
| Rifle | 82–87% |
| Shotgun | 86–88% |
| Sniper | 70–82% |

---

## 🔫 Weapon Arsenal

### Rifles
- **M4A4** — Balanced full-auto, low recoil
- **AK-47** — High damage, more recoil
- **M4A1-S** — Silenced, tight spread, smaller mag
- **FAMAS** — High RPM burst rifle
- **SG-553** — Mid-damage, scoped rifle

### SMGs
- **MP5-SD** — Silenced, fast fire rate
- **MAC-10** — Fastest RPM, loose spread
- **P90** — 50-round mag, reliable
- **UMP-45** — High damage SMG

### Shotguns
- **Nova** — 9 pellets, pump action, strong recoil
- **XM1014** — Semi-auto shotgun
- **MAG-7** — Tight spread, slowest pump

### Snipers
- **AWP** — 1-hit torso kill, heavy slow
- **SSG-08** — Scout rifle, faster movement
- **G3SG1** — Auto-sniper

### Pistols
- **Glock-18** — High mag, low damage
- **USP-S** — Silenced, tight spread
- **Desert Eagle** — High damage, strong recoil
- **Five-SeveN** — AP pistol, high mag
- **Tec-9** — Run-and-gun pistol

### Melee
- **Knife** — Fastest movement, 1-hit on close range, silent

---

## 🗺️ Map: GRID ARENA

The map is a large open arena (120×120 units) inspired by Rivals' flat, clean aesthetic with added verticality:

- **Grid floor** with glowing line overlays
- **4 elevated corner platforms** at height 4
- **Central raised platform** (2 units high)
- **Wall-jump corridor walls** along the X-axis
- **Floating mid platforms** for air control
- **Cover boxes** scattered around mid
- **4 tall corner pillars** for structure
- **Fog** at 80–200 units for atmosphere

---

## 🎮 Gameplay Features

- **CS2-style weapon buy menu** (`B`) with category tabs
- **Hitmarkers** with headshot color change
- **Kill feed** in top-right corner
- **Velocity bar** (bottom left)
- **Scope overlay** for sniper ADS
- **Screen shake** on shotgun fire
- **Weapon bob animation** while moving
- **ADS zoom** on all weapons (RMB)
- **Smooth reload animation**
- **Bullet tracers**
- **Hit particles** (orange = headshot)
- **Respawn system** (3s on death)
- **Enemy respawn** after 3s

---

## 🛠️ Tech Stack

- **Three.js r128** — 3D rendering
- **Vanilla JavaScript** — Game logic
- **HTML5 Canvas** — Scope overlay
- **CSS** — HUD and menus
- No build tools required — open `index.html` directly

---

## 🚀 Running Locally

```bash
git clone https://github.com/yourusername/arena-fps.git
cd arena-fps
# Open index.html in your browser, or serve with:
npx serve .
# or
python -m http.server 8080
```

Then open `http://localhost:8080` in Chrome or Firefox.

> **Note:** Pointer lock (mouse capture) requires a browser — won't work when opened as a raw `file://` path in some browsers due to security restrictions. Use a local server.

---

## 📁 Project Structure

```
arena-fps/
├── index.html        # Main game file (self-contained)
├── README.md         # This file
├── LICENSE           # MIT License
└── CONTRIBUTING.md   # Contribution guide
```

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to get involved.

Ideas welcome:
- Multiplayer via WebSockets
- More map geometry / map editor
- Sound effects (Web Audio API)
- Grenade/utility system
- Scoreboards
- Mobile touch controls

---

## 📄 License

MIT — see [LICENSE](LICENSE)
