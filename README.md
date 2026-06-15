# ⚔️ Echoes of the Unwritten

> *"In a world bound by script, every word… every action… is predetermined."*

A gothic web RPG where survival rewrites fate. Built entirely with vanilla HTML, CSS, and JavaScript — no frameworks, no build tools, just ink and shadow.

---

## 📖 Overview

**Echoes of the Unwritten** is a browser-based action RPG set in a void-black realm where reality fractures and glitches hide ancient truths. You play as a nameless figure trapped between the written and the unwritten, fighting through waves of corrupted enemies while uncovering a mysterious narrative — one surviving moment at a time.

The game features a hand-crafted pixel village silhouette backdrop, atmospheric particle effects, glitch animations, a WORD ability system, a boss encounter, and three distinct endings.

---

## 🎮 How to Play

### Controls

| Key | Action |
|-----|--------|
| `W` / `↑` | Move Up |
| `A` / `←` | Move Left |
| `S` / `↓` | Move Down |
| `D` / `→` | Move Right |
| `E` | Interact with NPCs |
| `F` | **BURN** — fire attack |
| `R` | **ERASE** — destroy ability |
| `ESC` | Pause / Close overlay |

### WORD System

As you progress, you unlock **WORDs** — special abilities tied to the game's narrative:

- `MOVE` — unlocked at start, enables player movement
- `BASIC` — unlocked early, enables basic attacks
- `BURN` — Phase 2 ability, fire blast in spread pattern
- `ERASE` — Phase 3 ability, digital zap attack

Each WORD is both a story beat and a gameplay unlock. The boss in Chapter 1 has three phases, each with a corresponding weakness word.

### Boss Fight (Chapter 1)

The boss encounter has **3 phases**:

| Phase | Weakness Word | Notes |
|-------|--------------|-------|
| 1 | `BASIC` | Standard attacks |
| 2 | `BURN` | Fire spread required |
| 3 | `ERASE` | Digital zap finisher |

Survive all three phases to reach **The Choice** — and your ending.

---

## 🌒 Endings

There are **three endings** based on your choices at the final decision point:

- **Restore** — The Script endures. Gold-toned resolution.
- **Destroy** — The Script burns. Red-toned conclusion.
- **Secret** — The hidden path. Cyan-tinted, unlocked under specific conditions.

All endings lead into a credits roll and a tease of **Chapter 2: The Awakening**.

---

## 🗂️ File Structure

```
echoes-of-the-unwritten/
├── main-menu.html      # Main menu with canvas background, overlays & game state
├── chapter1.html       # Full playable chapter — prologue through boss & endings
├── about.html          # Lore & game info page with GSAP scroll animations
└── README.md
```

> **Note:** Save data is stored in `localStorage` under the key `gamestate`. Clearing browser storage resets all progress.

---

## ✨ Features

- **Zero dependencies** — pure HTML/CSS/JS, runs in any modern browser
- **Canvas background** — procedurally drawn pixel village silhouette with moon, stars, fog, and mountains, redrawn on resize
- **Particle system** — 55 floating firefly/dust particles with pulse animations
- **Glitch FX** — randomized horizontal glitch lines burst across the canvas periodically
- **Custom cursor** — `✒` quill that morphs to `◆` on interactive elements
- **Wipe transitions** — cinematic scaleX wipe + color flash between pages
- **GSAP ScrollTrigger** — scrubbed scroll animations on the About page (cards, headings, feature list, CTA)
- **Responsive design** — hamburger nav on mobile, fluid typography via `clamp()`, adaptive grids
- **Keyboard navigation** — full arrow key + Enter support on the main menu
- **Persistent save** — `localStorage` tracks chapter, phase, HP, words, and playtime

---

## 🛠️ Running Locally

No build step needed. Just open any HTML file in your browser:

```bash
# Option 1 — open directly
open main-menu.html

# Option 2 — serve with Python (avoids some asset loading quirks)
python3 -m http.server 8080
# then visit http://localhost:8080/main-menu.html

# Option 3 — VS Code Live Server extension
# Right-click main-menu.html → "Open with Live Server"
```

---

## 🎨 Design System

All pages share a unified design language defined in CSS custom properties:

| Variable | Value | Use |
|----------|-------|-----|
| `--void` | `#04040a` | Page background |
| `--ink` | `#08080f` | Panel background |
| `--parchment` | `#e8dfc8` | Body text |
| `--gold` | `#c9a84c` | Primary accent |
| `--gold-bright` | `#f0d060` | Hover / highlight |
| `--gold-dim` | `#6a5022` | Subtle accents & borders |
| `--red-bright` | `#cc2233` | Enemy accents & danger |

**Fonts:** [UnifrakturMaguntia](https://fonts.google.com/specimen/UnifrakturMaguntia) · [Cinzel](https://fonts.google.com/specimen/Cinzel) · [Crimson Pro](https://fonts.google.com/specimen/Crimson+Pro)

**Animation library:** [GSAP 3.12.2](https://greensock.com/gsap/) + ScrollTrigger (About page only, via CDN)

---

## 👥 Credits

| Role | Name |
|------|------|
| Game Design & Story | Cherry Casires |
| Lead Dev / Creative Director | Radcliffe Abellana |
| Lead Illustrator & UI | Jade Alivio |
| Animation Specialist | Ziggy Bonsubre |

---

## 📄 License

This project is made for educational and creative purposes.
All original code, design, and narrative content © 2026 Echoes of the Unwritten team.

---

<div align="center">
  <em>"Once, I wanted freedom. Now… I decide fate."</em>
</div>
