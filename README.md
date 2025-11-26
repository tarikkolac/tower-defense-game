# 🏰 Tower Defense - Goblin Invasion

A pixel art tower defense game built with GDevelop game engine. Defend your castle against waves of goblin invaders!

![Game Banner](https://img.shields.io/badge/GDevelop-5.4-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Status](https://img.shields.io/badge/Status-Playable-brightgreen)

## 📖 Description

Tower Defense - Goblin Invasion is a classic tower defense game featuring:
- **10 unique goblin enemy types** with different abilities, speeds, and HP
- **3 tower types** (Archer, Mortar, Barracks) each with **3 upgrade levels**
- **10 challenging waves** with increasing difficulty
- **Strategic grid-based tower placement**
- **Pixel art graphics** with a fantasy theme
- **Sound effects** for immersive gameplay

## 🎮 How to Play

### Opening in GDevelop
1. Download and install [GDevelop](https://gdevelop.io/) (free and open-source)
2. Open GDevelop and click "Open a project"
3. Navigate to this folder and select `game.json`
4. Click the ▶️ Play button to start the game

### Game Controls
- **Left Click** on tower buttons to select a tower type
- **Left Click** on a tower spot (green squares) to build the selected tower
- **Play Button** starts the next wave
- **Pause Button** pauses/resumes the game

### Objective
- Prevent goblins from reaching your castle
- You start with **20 lives** and **200 gold**
- Each enemy that reaches the castle costs **1 life**
- Kill enemies to earn **gold** for building more towers
- Survive all **10 waves** to win!

## 🗼 Towers

### 🏹 Archer Tower
| Level | Damage | Range | Fire Rate | Cost |
|-------|--------|-------|-----------|------|
| 1 | 10 | 150px | 0.8s | 50 |
| 2 | 18 | 180px | 0.6s | +75 |
| 3 | 30 | 220px | 0.4s | +100 |

*Single target, fast attack speed*

### 💥 Mortar Tower
| Level | Damage | Range | AOE | Fire Rate | Cost |
|-------|--------|-------|-----|-----------|------|
| 1 | 25 | 200px | 50px | 2.0s | 80 |
| 2 | 45 | 230px | 70px | 1.7s | +100 |
| 3 | 70 | 260px | 90px | 1.4s | +130 |

*Area damage, slow fire rate*

### ⚔️ Barracks
| Level | Soldier HP | Damage | Soldiers | Cost |
|-------|------------|--------|----------|------|
| 1 | 50 | 8 | 2 | 70 |
| 2 | 80 | 14 | 3 | +90 |
| 3 | 120 | 22 | 4 | +120 |

*Spawns soldiers that block and fight enemies*

## 👾 Enemies

| Enemy | HP | Speed | Gold Reward | Special |
|-------|-----|-------|-------------|---------|
| Goblin Scout | 30 | Fast | 10 | Fastest, weakest |
| Goblin Warrior | 50 | Normal | 15 | Balanced |
| Goblin Brute | 100 | Slow | 25 | Tank type |
| Goblin Archer | 40 | Normal | 12 | Medium durability |
| Goblin Shaman | 35 | Slow | 20 | Heals nearby allies |
| Goblin Bomber | 25 | Fast | 18 | Explodes on death |
| Goblin Rider | 45 | Very Fast | 22 | Wolf mount |
| Goblin Tank | 150 | Very Slow | 35 | Most durable |
| Goblin Assassin | 30 | Fast | 28 | Can become invisible |
| Goblin Chieftain | 80 | Normal | 30 | Buffs nearby allies |

## 📂 Project Structure

```
tower-defense-game/
├── game.json                 # Main GDevelop project file
├── README.md                 # This file
├── assets/
│   ├── sprites/
│   │   ├── enemies/          # 10 goblin sprites (32x32)
│   │   ├── towers/           # 9 tower sprites (3x3 levels)
│   │   ├── projectiles/      # Arrow, mortar shell, explosion
│   │   ├── soldiers/         # 3 soldier level sprites
│   │   ├── map/              # Grass, path, tower spot, castle
│   │   └── ui/               # UI elements, buttons, panels
│   └── sounds/
│       └── effects/          # All sound effects
└── export/
    └── index.html            # Web export landing page
```

## 🌐 Web Export

To export for web:
1. Open the project in GDevelop
2. Go to **File > Export > Web (upload online)**
3. Follow the export wizard
4. Upload the generated files to any web server

The `export/index.html` file provides a landing page for the exported game.

## 🎨 Assets

All sprites are **32x32 pixel art** created specifically for this game:
- Fantasy color palette
- Distinct visual design for each enemy and tower type
- UI elements matching the game theme

Sound effects include:
- Arrow shot
- Explosion
- Sword hit
- Enemy death
- Tower build
- Coin pickup
- Wave start
- Game over
- Victory

## 🛠️ Development

### Requirements
- [GDevelop 5.4+](https://gdevelop.io/)

### Modifying the Game
- Open `game.json` in GDevelop
- Modify scenes, objects, events as needed
- Preview changes with the Play button
- Save your changes

### Adding New Content
- **New enemies**: Add sprite to `assets/sprites/enemies/`, create object in GDevelop
- **New towers**: Add sprite to `assets/sprites/towers/`, create object with variables
- **New waves**: Modify wave spawning events in the Game scene

## 📜 License

This project is open source and available under the MIT License.

## 🙏 Credits

- Built with [GDevelop](https://gdevelop.io/)
- Pixel art created with Python PIL
- Sound effects generated programmatically

---

**Enjoy defending your castle! 🏰⚔️**
