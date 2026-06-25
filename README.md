# 🎆 Particle Playground

Interactive 3D particle playground with 5 visual modes and music-reactive particles. Built with Three.js and the Web Audio API.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

## ✨ Features

- **5 Visual Modes** — Vortex, Gravity, Explosion, Aurora, Nebula
- **Music Reactive** — Particles pulse and dance to "Never Gonna Give You Up" via Web Audio API
- **Real-time Settings** — Adjust speed, particle size, brightness, and music reactivity on the fly
- **Keyboard Controls** — Switch modes, pause/unpause with keyboard shortcuts
- **Reset Button** — One-click reset to default settings
- **Three.js Powered** — Hardware-accelerated 3D particle rendering with custom GLSL shaders
- **Zero Dependencies** — No build step, no server needed
- **Responsive** — Works on desktop and mobile browsers

## 🎯 Modes

| Mode | Description |
|------|-------------|
| **Vortex** | Particles swirl in a dynamic spiral vortex |
| **Gravity** | Particles orbit a central gravitational point |
| **Explosion** | Particles burst outward with bass-triggered impulses |
| **Aurora** | Particles flow like aurora borealis ribbons |
| **Nebula** | Particles form colorful nebula-like clouds |

## 🎮 Controls

### Keyboard

| Key | Action |
|-----|--------|
| `1`-`5` | Switch visual mode |
| `Space` | Pause/resume particles |
| Mouse | Move cursor to interact with particles |

### Settings Panel (left sidebar)

| Slider | Range | Default | Description |
|--------|-------|---------|-------------|
| **Speed** | 0.5× – 3.0× | 1.0× | Overall animation speed |
| **Size** | 0.2× – 3.0× | 1.0× | Particle size multiplier |
| **Brightness** | 0% – 100% | 100% | Particle glow intensity |
| **Music React** | 0% – 100% | 70% | How strongly music affects particle behavior |

### Bottom Bar

| Button | Description |
|--------|-------------|
| **Vortex / Gravity / Explosion / Aurora / Nebula** | Switch visual mode |
| **⏸ Pause / ▶ Play** | Pause or resume particle animation |
| **🎵 Play Music / 🎵 Stop** | Toggle "Never Gonna Give You Up" |
| **↻ Reset** | Restore all settings to defaults |

## 🚀 Quick Start

This is a static site — no build step required!

```bash
# Clone the repo
git clone https://github.com/kamalcr7/particle-playground.git

# Open in browser
cd particle-playground
# Just open index.html in your browser, or serve with any static server:
python3 -m http.server 8080
```

Place an MP3 file at `assets/music/` and update `MUSIC_URL` in `index.html` to point to your song, or use the included bundled track.

## 🛠️ Tech Stack

- **Three.js** — 3D particle rendering via CDN (ESM modules) with custom GLSL shaders
- **Web Audio API** — `AnalyserNode` for real-time frequency analysis driving particle reactivity
- **Vanilla JavaScript** — No framework or build tools

## 📄 License

MIT
