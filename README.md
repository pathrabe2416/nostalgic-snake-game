# 🐍 Nostalgic Snake

A visually immersive Snake game built with pure **HTML**, **CSS**, and **Vanilla JavaScript** — no frameworks, no libraries, no dependencies.

Designed with a **modern dark aesthetic**, smooth canvas-rendered animations, adaptive layouts, and responsive touch support — delivering a polished arcade-style experience directly in the browser.

---

## 🔗 Live Demo

**[▶ Play Now → pathrabe2416.github.io/nostalgic-snake-game](https://pathrabe2416.github.io/nostalgic-snake-game/)**

---

## 🚀 Overview

Nostalgic Snake is a love letter to classic arcade gaming — rebuilt with modern front-end craft. It runs entirely on `<canvas>`, scales fluidly across every screen size and orientation, and supports both keyboard and touch input with equal polish.

The application emphasizes:

- Pixel-perfect canvas rendering with glow and shine effects
- Adaptive layout engine that responds to device type and orientation
- Smooth performance at variable tick speeds
- Zero external dependencies — pure front-end execution

---

## 🧠 Core Features

### 🎮 Game Mechanics

- Classic Snake gameplay — eat food, grow longer, avoid yourself
- **Wall-wrap mode** — snake passes through edges and re-enters from the opposite side
- **Progressive speed** — game accelerates as your score climbs, capped at a minimum interval for fairness
- Self-collision detection for a precise game-over condition

### 🎨 Visual System

- Canvas-rendered game board with a subtle dot grid
- **Animated snake head** — glowing yellow-green fill with directional shine strip and blinking eyes that follow movement direction
- **Body fade gradient** — segments fade in opacity toward the tail for visual depth
- **Pulsing food** — sine-wave radius animation with radial glow and highlight shine
- **Eat flash** — brief canvas-wide tint on food pickup
- Smooth overlay transitions with `cubic-bezier` spring animations
- **New Best badge** — animated pill notification on high score

### 📐 Adaptive Layout Engine

The layout engine recalculates the entire grid on every resize and orientation change:

- Detects pointer type (touch vs. mouse) and orientation (portrait vs. landscape)
- Computes optimal cell size, column count, and row count to fill available space
- Switches CSS grid layout between portrait and landscape modes automatically
- D-pad is shown only on touch devices; hidden on desktop
- Landscape touch mode relocates the score panel alongside the D-pad

### 📊 Score System

- Live score tracking with animated pop effect on increment
- Persistent **best score** tracking across the session
- Score, best, and snake length displayed in the HUD at all times
- Game-over overlay shows contextual title based on score (`"Nice Try"` → `"Impressive"`)

### 📱 Responsive Design

Fully optimized for:

- Desktop (keyboard)
- Tablet (touch + landscape)
- Mobile (portrait + landscape)

Uses `clamp()`, `env(safe-area-inset-*)`, and dynamic CSS variable recalculation to maintain proportional board sizing on every device.

---

## 🕹 How to Play

1. Open the [live demo](https://pathrabe2416.github.io/nostalgic-snake-game/)
2. Press **Space**, **Enter**, or **tap** to start
3. Guide the snake to eat the red food pellets
4. Each pellet grows your snake and increases your score
5. The game ends if the snake collides with itself

---

## 🎛 Controls

| Input | Action |
|---|---|
| `↑ ↓ ← →` / `W A S D` | Steer the snake |
| `Space` / `Enter` | Start / Restart |
| **Swipe** | Steer on touch devices |
| **D-pad** | On-screen directional buttons (touch only) |

> Reverse direction is blocked — you cannot steer directly into yourself.

---

## 🛠 Tech Stack

| Layer | Detail |
|---|---|
| **HTML5** | Semantic structure, canvas element, overlay system |
| **CSS3** | Grid layout, CSS variables, keyframe animations, safe-area support |
| **Vanilla JS** | Game loop, canvas rendering, input handling, layout engine |
| **Canvas 2D API** | All game graphics — snake, food, grid, effects |

No frameworks. No libraries. Pure front-end execution.

---


## 🏆 Highlights

- ✔ Fully canvas-rendered — no DOM elements for game objects
- ✔ Directional snake eyes that update with movement
- ✔ Adaptive grid that fills the screen on any device
- ✔ Touch-first D-pad with landscape mode score panel
- ✔ No build tools, no bundler — open `index.html` and it runs
- ✔ Production-level UI polish on a zero-dependency codebase

---


## ⭐ Support

If you appreciate the design or architecture:

- ⭐ **Star the repository**
- 🍴 **Fork and experiment**
- 🚀 **Improve the AI / add new features**

Contributions are welcome.

---

## 📄 License

MIT — free to use, modify, and distribute.
