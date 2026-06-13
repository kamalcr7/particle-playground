# 🎆 Particle Playground

Interactive 3D particle playground with 5 visual modes and music-reactive particles. Built with Three.js and the Web Audio API.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

## ✨ Features

- **5 Visual Modes** — Vortex, Gravity, Explosion, Aurora, Nebula
- **Music Reactive** — Particles dance to synthesized electronic music via Web Audio API
- **Keyboard Controls** — Switch modes, pause, toggle music with keyboard shortcuts
- **Three.js Powered** — Hardware-accelerated 3D particle rendering
- **Zero Dependencies** — No build step, no server needed
- **Responsive** — Works on desktop and mobile browsers

## 🎯 Modes

| Mode | Description |
|------|-------------|
| **Vortex** | Particles swirl in a dynamic spiral vortex |
| **Gravity** | Particles orbit a central gravitational point |
| **Explosion** | Particles burst outward in explosive patterns |
| **Aurora** | Particles flow like aurora borealis ribbons |
| **Nebula** | Particles form colorful nebula-like clouds |

## 🎮 Controls

| Key | Action |
|-----|--------|
| `1`-`5` | Switch visual mode |
| `Space` | Pause/resume particles |
| `M` | Toggle music on/off |
| Mouse | Interact with particles |

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

## 📦 Deployment

### Cloudflare Pages

```bash
npx wrangler pages deploy . --project-name particle-playground --branch main
```

### Any Static Host

Just upload the `index.html` file to any static hosting service (GitHub Pages, Netlify, Vercel, etc.).

## 🛠️ Tech Stack

- **Three.js** — 3D particle rendering via CDN (ESM modules)
- **Web Audio API** — Synthesized music generation and analysis
- **Vanilla JavaScript** — No framework or build tools

## 📄 License

MIT
