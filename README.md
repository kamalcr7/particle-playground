# 🎆 Particle Playground

Interactive 3D particle playground with 6 visual modes, music-reactive particles, and physics-based interactions. Built with Three.js, custom GLSL shaders, and the Web Audio API.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

## ✨ Features

- **6 Visual Modes** — Vortex, Gravity, Explosion, Aurora, Nebula, and the legendary Rick Astley Dance Mode.
- **Music Reactive** — Particles pulse, dance, speed up, and vibrate in real-time to "Never Gonna Give You Up" via the Web Audio API.
- **Interactive Physics** — Precise mouse/touch 3D tracking:
  - **Gravity / Nebula**: Pulls particles into a gravitational singularity/black hole on click/touch.
  - **Explosion / Rickroll**: Disperses particles dynamically with shockwaves on click/touch or strong bass beats.
  - **Aurora**: Warps and swirls ribbons magnetically around the cursor.
- **Real-time Settings Sidebar** — Adjust speed, particle size, brightness, particle count, and music reactivity sensitivity on the fly.
- **Zero Garbage Collection (GC) Overhead** — Highly optimized rendering utilizing in-place color algorithms. Prevents browser frame drops and micro-stutters.
- **Responsive Design** — Elegant, responsive glassmorphism HUD that adapts seamlessly to desktop and mobile displays.
- **Zero Dependencies** — Runs directly in any modern browser without compilers, bundlers, or servers.

---

## 🎯 Modes

| Mode | Description |
|------|-------------|
| **Vortex** | Particles swirl in a dynamic, high-velocity spiral vortex. |
| **Gravity** | Particles orbit a central gravity point, reacting with explosive shockwaves on mouse-clicks and audio beats. |
| **Explosion** | A high-definition contained sphere where particles expand in crisp shockwave rings and snap back quickly. |
| **Aurora** | Fluid, smooth aurora borealis ribbons that swirl magnetically around your cursor. |
| **Nebula** | A beautiful dual-arm spiral galaxy featuring differential rotation, a black-hole gravity core, and a wide HSL rainbow spectrum. |
| **Rick Astley** | A custom, slimmed-down 3D particle silhouette of Rick Astley that performs 4 continuous choreographed dance routines (Classic Sway, Shoulder Shimmy, Arm Wave, Foot Shuffle) with smooth cross-fading, complete with a mic stand and skin-toned hands. |

---

## 🎮 Controls

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `1` – `6` | Switch visual modes (6 = Rick Astley Mode) |
| `Space` | Pause / resume particles |
| Mouse / Touch | Move cursor to interact (warp, drag, or explode particles) |

### Settings Panel (left sidebar)

| Control | Range | Default | Description |
|---------|-------|---------|-------------|
| **Speed** | 0.5× – 3.0× | 1.0× | Overall animation speed multiplier |
| **Size** | 0.2× – 3.0× | 1.0× | Base particle sizing |
| **Brightness** | 0% – 100% | 100% | Particle glow intensity (adjusts custom GLSL shader values) |
| **Music React** | 0% – 100% | 70% | Depth of audio-reactive size pulses |
| **Particle Count** | 100 – 16,000 | 12,000 | Total active rendering budget (dynamic buffer updates) |

---

## 🚀 Quick Start

Since this is a static project, no build steps are required! 

```bash
# Clone the repository
git clone https://github.com/kamalcr7/particle-playground.git

# Navigate to the folder
cd particle-playground

# Run a static server to bypass browser CORS limitations for audio loading:
# Using Python:
python -m http.server 8080

# Or using Node.js:
npx http-server -p 8080
```
Open `http://localhost:8080` in your web browser.

---

## 🛠️ Tech Stack

- **Three.js** — GPU-accelerated particle system loaded via ESM modules.
- **Web Audio API** — Real-time `AnalyserNode` with an attack-release envelope follower for smooth music reactivity.
- **Custom GLSL Shaders** — Custom vertex and fragment shaders for high-performance size attenuation, color blends, and crisp brightness scaling.
- **Vanilla JS & CSS** — Glassmorphic styling and interactive settings panel.

## 📄 License

MIT
