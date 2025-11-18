# Territory Control - RPS Strategy Game

A fast-paced, turn-based strategy game where you compete against an AI opponent to control the most territory using Rock-Paper-Scissors combat mechanics.

## 🎮 How to Play

1. **Open the Game**: Simply open `index.html` in any modern web browser
2. **Select a Unit**: Click on one of the three unit types (Warrior, Archer, or Mage)
3. **Place Units**: Click on empty tiles or your own territory to place units
4. **Combat**: Units automatically battle adjacent enemies using RPS rules
5. **Win**: Control 60% of the map or eliminate your opponent

## 🎯 Game Mechanics

### Unit Types & Combat

- **⚔️ Warriors (Red)**: Beat Archers, lose to Mages
- **🏹 Archers (Green)**: Beat Mages, lose to Warriors
- **🔮 Mages (Blue)**: Beat Warriors, lose to Archers

### Turn Structure

- Place 1-3 units per turn
- Units can be placed on:
  - Empty tiles adjacent to your territory
  - Your own territory (if no unit is there)
- Click "End Turn" when finished
- AI takes its turn automatically

### Combat System

- When you place a unit, it automatically battles all adjacent enemy units
- Winner converts the enemy tile to their color
- Battles can chain-react across the map
- Strategic placement is key!

## ⚙️ Settings

### Map Sizes
- **Small**: 10x10 grid (quick games, ~5 minutes)
- **Medium**: 15x15 grid (balanced, ~7 minutes) - Default
- **Large**: 20x20 grid (epic battles, ~10 minutes)

### AI Difficulty
- **Easy**: Places 1-2 units randomly
- **Medium**: Places 2-3 units with basic strategy - Default
- **Hard**: Places 3 units with advanced tactics

### AI Strategy
- **Defensive**: Protects its territory, rarely attacks
- **Balanced**: Mix of defense and offense - Default
- **Aggressive**: Constantly attacks player territory

## 🎨 Features

✅ Clean, colorful tile-based graphics
✅ Smooth battle animations
✅ Real-time territory percentage display
✅ Undo last move (during your turn)
✅ Restart game anytime
✅ Responsive design
✅ 60fps animations
✅ Victory/defeat screens

## 🎓 Strategy Tips

1. **Counter Your Opponent**: Watch what units the AI uses and place counters
2. **Protect Borders**: Defend tiles adjacent to enemy territory
3. **Chain Reactions**: A well-placed unit can trigger multiple battles
4. **Expand Wisely**: Don't spread too thin - consolidate territory
5. **Use All Units**: Each turn you can place up to 3 units - use them!

## 🛠️ Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Rendering**: HTML5 Canvas
- **Styling**: Tailwind CSS (CDN)
- **File Size**: Single HTML file (~20KB)
- **Performance**: 60fps smooth animations
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

## 🚀 Quick Start

```bash
# Clone or download the repository
cd territory-control-game

# Open in browser
open index.html
# or
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## 📝 Game Rules Summary

1. Players alternate turns (Player → AI → Player)
2. Place 1-3 units per turn on valid tiles
3. Units fight adjacent enemies automatically
4. RPS combat: Warrior > Archer > Mage > Warrior
5. Winner takes the enemy tile
6. First to 60% territory wins (or eliminate opponent)

## 🎯 Win Conditions

- Control **60% or more** of the total map tiles
- **Eliminate** all enemy units and territory
- AI surrenders if it has no valid moves

## 🔄 Controls

- **Select Unit**: Click unit buttons on left panel
- **Place Unit**: Click on valid tiles (highlighted on hover)
- **End Turn**: Click "End Turn" button
- **Undo**: Click "Undo Move" (only during your turn)
- **Restart**: Click "Restart Game" anytime
- **Settings**: Change map size, AI difficulty, and strategy

## 📊 UI Elements

- **Territory Bars**: Real-time % control for Player (blue) and AI (red)
- **Turn Display**: Shows whose turn it is
- **Units Left**: Remaining units you can place this turn
- **Unit Info**: Shows RPS relationships for each unit type

## 🎮 Game Flow

```
Start Game
    ↓
Player Turn (place 1-3 units)
    ↓
Battles Resolve Automatically
    ↓
Check Win Condition
    ↓
AI Turn (AI places units)
    ↓
Battles Resolve
    ↓
Check Win Condition
    ↓
Back to Player Turn
    ↓
Game Over (Victory/Defeat)
```

## 🐛 Known Limitations

- No save/load game feature
- No multiplayer (single player vs AI only)
- No sound effects (visual only)
- No mobile touch optimization (works but not ideal)

## 📜 License

Free to use and modify. Created as a strategy game demo.

## 🎉 Enjoy!

Have fun conquering territory and outsmarting the AI! Try different strategies and difficulty levels to master the game.
