<h1 align="center">EDILAS: The Living Pilgrimage</h1>
<p align="center"><strong>A dark survival RPG where every death reshapes the world</strong></p>

<p align="center">
  <a href="https://stabrea.github.io/edilas-game/"><img src="https://img.shields.io/badge/▶_Play_Now-00ff88?style=for-the-badge&logoColor=black" alt="Play Now"/></a>
</p>

---

### About

EDILAS is a browser-based dark survival RPG built from scratch with **TypeScript**, **Phaser 3**, and **bitECS** (Entity Component System). The game features procedural world generation, real-time combat, a paper-doll character system, and persistent world state.

### Technical Highlights

| Metric | Value |
|--------|-------|
| Source Modules | 98 |
| Test Suite | 1,425 tests across 37 files |
| Game Systems | 37+ (AI, combat, weather, inventory, crafting, dialogue, etc.) |
| Architecture | Entity Component System (bitECS) |
| Rendering | Phaser 3 WebGL |
| Build | Vite + TypeScript |
| CI/CD | Auto-deployed from private source repo via GitHub Actions |

### Key Systems

- **Procedural World Generation** — Biome-based terrain with dynamic weather affecting gameplay
- **Real-Time Combat** — Melee/ranged with dodge, parry, critical hits, and backstab mechanics
- **Boss Imprint System** — Absorb defeated boss powers (Valheim-inspired)
- **Weapon Echo System** — Kill combos charge phantom strikes (Dead Cells-inspired)
- **Quirk System** — Behavioral traits evolve based on playstyle (Darkest Dungeon-inspired)
- **Paper-Doll Characters** — Layered sprite system with 135+ real sprites
- **Day/Night Cycle** — Dynamic lighting with gameplay consequences
- **Full Save System** — Serialize/deserialize complete world state

### Architecture

The source code lives in a private repository. This public repo contains only the production build, auto-deployed via GitHub Actions on every push.

```
Private Repo (stabrea/EDILAS)
  └── push to master
       └── GitHub Actions: npm ci → tsc → vite build
            └── Deploy dist/ to this repo
                 └── GitHub Pages serves the game
```

---

<p align="center"><em>Built by <a href="https://github.com/stabrea">Taofik Bishi</a></em></p>
<p align="center"><em>© 2026 All rights reserved</em></p>
