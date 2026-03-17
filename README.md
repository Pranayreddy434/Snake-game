# 🐍 Snakes & Ladders

A fully featured, browser-based **Snakes & Ladders** game built with pure **HTML, CSS, and JavaScript** — no frameworks, no dependencies (except Bootstrap for layout). Play solo against a bot or challenge a friend in two-player mode, across three uniquely designed boards.

![Game Preview](https://img.shields.io/badge/Game-Snakes%20%26%20Ladders-brightgreen?style=for-the-badge&logo=github)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

---

## 🎮 Live Demo

> Deploy this repo on Netlify or GitHub Pages to get a live link.  
> See [Deployment](#-deployment) section below.

---

## ✨ Features

### 🎲 Real 3D Dice
- Each player has their own **color-coded physical dice** — red for Player 1, blue for Player 2
- Dice animate with a 3D tumbling rotation on every roll
- Active dice glows to indicate whose turn it is
- Inactive dice is greyed out and unclickable

### 🗺️ Three Unique Boards per Difficulty
| Difficulty | Snakes | Ladders | Theme |
|------------|--------|---------|-------|
| 😊 Easy    | 3 short snakes | 6 long ladders | Green board — very forgiving |
| 😤 Moderate | 5 snakes | 4 ladders | Amber board — balanced challenge |
| 💀 Hard    | 8 snakes (including one near 96!) | 3 ladders only | Red board — brutal |

### 🎯 Exact Roll to Win Rule
- You must roll **exactly** the number needed to land on 100
- If you overshoot (roll more than needed) → your turn is **skipped**, no movement
- A yellow warning message shows: `"Need X to win, got Y — turn skipped!"`
- Status bar dynamically shows the exact number needed when within 6 squares of 100

### 🤖 Smart Bot (Solo Mode)
- Bot **auto-rolls** its dice — no button press needed
- Bot thinking delay varies by difficulty:
  - Easy → 1.9s delay (slow)
  - Moderate → 1.3s delay
  - Hard → 0.75s delay (fast)

### 🐍 Real Drawn Snakes & Ladders
- Snakes are drawn using **Canvas API** with sinusoidal wavy bodies, gradients, scale patterns, green heads with yellow eyes, forked tongues, and tail tips
- Ladders are drawn with two golden rails, evenly spaced rungs, shine highlights, and round end caps — all rendered in HTML5 Canvas

### 📐 Dice Layout by Game Mode
- **Solo mode** — both dice appear side-by-side **below** the board
- **Two-player mode** — Player 1's dice sits **above** the board, Player 2's dice sits **below** — each player faces their own die

### 🏠 Back to Menu
- A **Menu button** during gameplay opens a confirmation modal
- Safely returns to the start screen without accidental loss of game
- Full state and board is reset cleanly on return

### 🏆 Other Features
- Step-by-step animated player movement
- Snake slide / ladder climb animations with glow pulses
- Per-round scoreboard that persists across rounds
- Match history log (newest first)
- Confetti celebration on win
- Fully responsive — works on mobile, tablet, and desktop
- No page reloads needed — entire game runs in a single HTML file

---

## 🕹️ How to Play

1. Choose **Solo vs Bot** or **Two Players**
2. Select a **difficulty** (Easy / Moderate / Hard)
3. Click **Start Game**
4. **Click your dice** to roll on your turn
5. Move along the board — land on a ladder to climb up, land on a snake to slide down
6. First player to land **exactly on 100** wins!
7. If you roll more than needed to reach 100, your turn is skipped

---

## 📁 Project Structure

```
Snake-game/
│
└── index.html        ← Entire game (HTML + CSS + JS in one file)
```

This is a single-file project — everything lives in `index.html`. No build tools, no npm, no compilation needed.

---

## 🚀 Deployment

### Option 1 — Netlify Drag & Drop (Fastest)
1. Go to [netlify.com](https://netlify.com) and sign in
2. Go to **Sites → drag and drop your site folder here**
3. Drop a folder containing `index.html`
4. Get a live URL instantly (e.g. `https://snake-game-xyz.netlify.app`)

### Option 2 — Netlify via GitHub (Auto-deploy)
1. Push this repo to GitHub
2. Go to Netlify → **Add new site → Import from Git**
3. Select this repository
4. Set publish directory to `/` (root)
5. Click **Deploy** — every push auto-deploys

### Option 3 — GitHub Pages
1. Go to your repo **Settings → Pages**
2. Set source to `main` branch, folder `/` (root)
3. Save — GitHub will publish at `https://yourusername.github.io/Snake-game/`

### Option 4 — Run Locally
Just open the file in any browser:
```bash
git clone https://github.com/Pranayreddy434/Snake-game.git
cd Snake-game
open index.html       # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

No server required. No dependencies to install.

---

## 🛠️ Built With

| Technology | Purpose |
|------------|---------|
| HTML5 | Game structure and layout |
| CSS3 | Animations, 3D dice, themes, responsive design |
| Vanilla JavaScript | All game logic, state management |
| HTML5 Canvas API | Drawing real snakes and ladders |
| Bootstrap 5 | Grid layout and utility classes |
| Google Fonts | Fredoka One + Nunito typefaces |

---

## 🎨 Game Screenshots

> *(Add your own screenshots here after deployment)*

| Start Screen | Easy Board | Hard Board |
|---|---|---|
| ![start](#) | ![easy](#) | ![hard](#) |

---

## 📋 Game Rules Summary

| Situation | Result |
|-----------|--------|
| Land on a ladder bottom | Climb to the top |
| Land on a snake head | Slide to the tail |
| Roll exactly the number to reach 100 | 🏆 Win! |
| Roll more than needed for 100 | Turn skipped, no move |
| Bot's turn (Solo mode) | Bot rolls automatically |

---

## 🤝 Contributing

Pull requests are welcome! Here are some ideas for improvement:
- Add sound effects
- Add player name customization
- Add a 4-player mode
- Add an online multiplayer mode
- Add different board sizes (e.g. 8×8)

---

## 👨‍💻 Author

**Pranay Reddy**  
GitHub: [@Pranayreddy434](https://github.com/Pranayreddy434)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Made with ❤️ using HTML, CSS & JavaScript*
