# Neon Runner 🌃⚡

A fast-paced, neon-themed endless runner built as a single HTML file using **HTML, CSS, and vanilla JavaScript**. Jump, double-jump, slide, collect coins, use power-ups, and survive an increasingly fast stream of obstacles while chasing a new high score.

## ✨ Features

- 🎮 **Endless runner gameplay** with continuously generated obstacles, coins, power-ups, and environmental effects.
- 🦾 **Responsive player controls** with jumping, double-jumping, sliding, and mid-air diving.
- 💥 **Multiple obstacle types** including blocks, spikes, saws, crystals, and high-speed drones.
- 🪙 **Coin + combo scoring system** where consecutive coin pickups increase the score multiplier.
- 🛡️ **Four power-ups**
  - **Shield** — blocks an obstacle collision.
  - **Magnet** — pulls nearby coins toward the player.
  - **Slow-Mo** — temporarily reduces the gameplay speed.
  - **2x Score** — doubles coin score gains while active.
- 🎚️ **Four difficulty modes**
  - **Easy** — 5 lives, slower starting pace, 0.75× score.
  - **Normal** — 3 lives, balanced pace, 1× score.
  - **Hard** — 2 lives, faster and denser gameplay, 1.5× score.
  - **Insane** — 1 life, very fast gameplay, 2.25× score.
- 🌌 **Dynamic neon environments** that transition through:
  - Night City
  - Purple Dawn
  - Toxic Green
  - Solar Flare
- 🌠 **Canvas-based visual effects** including particles, motion trails, meteors, glowing elements, reflections, scanlines, screen shake, and atmospheric effects.
- 🔊 **Built-in sound effects** using the browser Web Audio API, with mute/unmute control.
- 💾 **Persistent best scores** stored locally in the browser for each difficulty level.
- 📊 **Game-over statistics** showing difficulty, distance, coins collected, maximum combo, time, score multiplier, and best-score status.
- 📱 **Mobile/touch support** with on-screen Jump and Slide controls.
- ⏸️ **Pause/resume support** using the UI button or keyboard.
- ⚡ **Performance-conscious rendering** with capped device-pixel-ratio scaling and cached visual effects.

## 🎮 Controls

### Desktop

| Action | Controls |
|---|---|
| Jump / Double-Jump | `Space` / `↑` / `W` / Mouse Click |
| Slide | `↓` / `S` |
| Pause / Resume | `P` / `Esc` |
| Mute / Unmute | `M` |

### Mobile

Use the on-screen **JUMP** and **SLIDE** buttons displayed on touch devices.

## 🧠 Gameplay

The goal is simple: **survive for as long as possible and achieve the highest score**.

The game continuously increases its speed, making obstacle timing more demanding as the run progresses. Missing an obstacle costs a life and resets the current combo. Collecting coins increases your combo and score multiplier, while power-ups can change the flow of a run.

Your best score is saved separately for each selected difficulty using browser `localStorage`.

## 🎚️ Difficulty System

| Difficulty | Lives | Starting Speed | Score Multiplier |
|---|---:|---:|---:|
| Easy | 5 | 6 | 0.75× |
| Normal | 3 | 7 | 1× |
| Hard | 2 | 8.2 | 1.5× |
| Insane | 1 | 9.4 | 2.25× |

Higher difficulties also increase the rate at which the game becomes faster and reduce the spacing between obstacles.

## 🪙 Scoring & Combos

Coins are worth more as your combo grows. The combo multiplier increases every five consecutive coin pickups, up to a 5× combo multiplier.

The **2x Score** power-up multiplies coin scoring again while active.

A run also awards a small amount of score for successfully passing obstacles.

## 🛠️ Tech Stack

- **HTML5**
- **CSS3**
- **Vanilla JavaScript**
- **HTML5 Canvas API**
- **Web Audio API**
- **Browser Local Storage**

No framework, package manager, build process, or external dependency is required.

## 🚀 Run Locally

Because the project is self-contained, you can run it directly in a browser.

### Option 1 — Open directly

1. Clone or download the repository.
2. Open `ankit.html` in a modern web browser.
3. Click **START RUN** and choose a difficulty.

### Option 2 — Use a local server

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

Then serve the folder with any static web server. For example, with Python:

```bash
python -m http.server 8000
```

Open:

```text
http://localhost:8000/ankit.html
```

## 📁 Project Structure

```text
.
└── ankit.html
```

The current version keeps the complete game in one HTML file, including:

- Interface markup
- Styling
- Game state
- Player physics
- Collision handling
- Procedural rendering
- Audio
- Difficulty settings
- Scoring
- Touch controls
- Game flow

## 🎨 Visual Style

Neon Runner uses a synthwave-inspired visual design with glowing cyan, purple, green, orange, and gold accents. The world includes a futuristic city skyline, mountains, stars, clouds, a glowing planet, a perspective grid, reflections, particles, and atmospheric post-processing effects.

## 🔧 Customization

The game is designed so the main gameplay systems can be modified directly inside the HTML file.

Examples of easy-to-edit areas:

- Difficulty values
- Player gravity and jump strength
- Obstacle spawn rates
- Coin spawn frequency
- Power-up durations
- Biome colors and themes
- Score multipliers
- Visual effects
- Sound frequencies and durations

## 📌 Browser Compatibility

The project is intended for modern browsers with support for:

- HTML5 Canvas
- `requestAnimationFrame`
- Web Audio API
- `localStorage`
- Pointer/touch input

## 📄 License

No license has been specified for this repository yet. Add a license file and update this section before distributing the project publicly.

---

⭐ If you enjoy the project, consider giving the repository a star and experimenting with the gameplay values to create your own version.
