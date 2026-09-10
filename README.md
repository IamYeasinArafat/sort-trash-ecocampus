# ♻️ Eco Campus Sorting Relay

A fast-paced, browser-based waste-sorting game built to train players to correctly sort everyday items into **Compost**, **Recyclables**, and **Non-Recyclables** — without cross-contaminating the bins.

Single HTML file, zero dependencies, zero build step. Open it and play.

![Mode](https://img.shields.io/badge/modes-2-brightgreen) ![Dependencies](https://img.shields.io/badge/dependencies-none-blue) ![Build](https://img.shields.io/badge/build%20step-none-lightgrey)

## 🎮 Play it

Open `eco-campus-sorting-relay.html` in any modern browser — no server, no install, no npm.

```bash
open eco-campus-sorting-relay.html      # macOS
xdg-open eco-campus-sorting-relay.html  # Linux
start eco-campus-sorting-relay.html     # Windows
```

Or just double-click the file.

## 🧠 Concept

Three color-coded campus bins each accept different waste:

| Bin | Accepts |
|---|---|
| 🟤 **Compost** | Flowers, food waste, wooden cutlery |
| 🟢 **Recyclables** | Glass, metal, paper, plastic (clean & dry only) |
| ⚫ **Non-Recyclables** | Styrofoam, chip bags, tissue paper, contaminated items |

Items fly at you one at a time. Sort each one into the right bin before time runs out. Get it wrong and you "contaminate" the bin — which costs you points and teaches you why.

## 🕹️ Gameplay modes

**Trash Auditor** — One shared timer. Sort as many items as you can before it hits zero.
- `+1` point per correct sort
- `−2` points per contamination

**Relay Sprint** — Each item gets its own countdown, like tagging in a relay. Chain correct sorts together to build a streak multiplier for bonus points. One miss and the streak resets.

## 👥 Crews (difficulty presets)

| Crew | Best for | Pace |
|---|---|---|
| 🧒 Kids Campus | Younger players | Longer timers, encouraging feedback |
| 🎓 Student Life | General/default | Balanced |
| 💼 Office Challenge | Workplace events | Shortest timers, "audit" framing |

## 🎯 Controls

- **Click / tap** a bin to sort the current item
- **Drag** the item card onto a bin
- **Keyboard**: `1` Compost · `2` Recyclables · `3` Non-Recyclables

## 📚 Built-in eco-education

Getting an item wrong (or right, for a few tricky ones) surfaces a short, contextual fact instead of a lecture at the end — for example:

- Why **wooden cutlery** goes in Compost, not Recycling
- Why **used tissue paper** can't be recycled
- Why **grease** (e.g. a used pizza box) contaminates paper recycling

The end screen recaps your score, accuracy, best streak, and contamination count.

## 🛠️ Tech stack

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools
- Fully responsive (desktop + mobile)
- Respects `prefers-reduced-motion`
- Keyboard-accessible bin controls

## 📁 Project structure

```
eco-campus-sorting-relay.html   # the entire game — markup, styles, and logic
README.md                       # this file
```

## ✏️ Customizing

All game content lives in a few config objects near the top of the `<script>` block:

- `ITEMS` — add/edit waste items, their emoji, correct bin, and optional educational fact
- `SQUADS` — tune timers and tone per audience
- `MODES` — adjust mode descriptions or scoring logic in `handleChoice()`

No build step required — edit and refresh.

## 🗺️ Roadmap ideas

- [ ] In-person relay mode with printable item cards + scorecard
- [ ] Multiplayer local mode (two players, split keyboard/bins)
- [ ] Leaderboard / shareable results
- [ ] Additional waste categories (e-waste, hazardous materials)

## 📄 License

MIT — use it, remix it, run it at your next campus or office sustainability event.
