# gridlock

A fast-paced browser-based first-person shooter built with Three.js.

![ARENA FPS](https://img.shields.io/badge/engine-Three.js%20r128-blue?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Web%20Browser-green?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-orange?style=flat-square)

---

## Controls

| Key | Action |
|-----|--------|
| `W A S D` | Move |
| `Space` | Jump |
| `Shift` | Sprint |
| `Ctrl` | Crouch |
| `LMB` | Shoot |
| `RMB` | ADS (Aim Down Sights) |
| `R` | Reload |
| `1` | Primary Weapon |
| `2` | Secondary / Pistol |
| `3` | Knife (fastest movement) |
| `B` | Open Weapon Menu |
| `Esc` | Unlock Mouse |

---

## Weapons

### Rifles
- **AK-47** — High damage, moderate recoil

### Pistols
- **Glock-18** — Large mag, low damage
- **Desert Eagle** — High damage, heavy recoil

### Melee
- **Knife** — Silent, fastest movement speed

---

## Movement

Heavier weapons slow you down. The knife gives the fastest movement. Sprint with `Shift` on the ground for a speed boost.

| Weapon Class | Speed |
|---|---|
| Knife | 115% |
| Pistol | 97–100% |
| SMG | 92–95% |
| Rifle | 85% |
| Shotgun | 86–88% |
| Sniper | 70% |

---

## Map

A large open arena (120×120 units) with a bright, clean look:

- Light gray floor and walls
- Central raised platform with cover boxes scattered around
- Corner pillars and elevated platforms for vertical play
- Wall-jump corridor walls along the X-axis
- 10 stationary target boards around the walls to shoot at

---

## Features

- Weapon selection menu (`B`) with category tabs
- Hitmarkers on target hits
- Kill feed in top-right corner
- Velocity bar (bottom left)
- Scope overlay for sniper ADS
- Weapon bob animation while moving
- Smooth reload animation
- Bullet decals that persist on surfaces
- Hit particles on impact

---

## Tech Stack

- **Three.js r128** — 3D rendering
- **Vanilla JavaScript** — Game logic
- **HTML5 Canvas** — Scope overlay
- **CSS** — HUD and menus
- No build tools required — open `index.html` in a browser

> **Note:** Pointer lock (mouse capture) requires a local server in some browsers. Running directly as a `file://` URL may not work due to security restrictions.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to get involved.

Ideas welcome:
- Sound effects (Web Audio API)
- More map geometry
- Multiplayer via WebSockets
- Mobile touch controls
- Scoreboards

---

## 📄 License

MIT — see [LICENSE](LICENSE)
