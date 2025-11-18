# Territory Control - RPS Strategy Game

A polished, fast-paced, turn-based strategy game where you compete against an AI opponent to control the most territory using Rock-Paper-Scissors combat mechanics.

## 🎮 How to Play

1. **Open the Game**: Simply open `index.html` in any modern web browser
2. **Select a Unit**: Click on one of the three unit types (Warrior, Archer, or Mage) or press 1, 2, or 3
3. **Place Units**: Click on tiles **adjacent to your territory** to place units (you must expand from your controlled area)
4. **Combat**: Units automatically battle adjacent enemies using RPS rules
5. **End Turn**: Click "End Turn" or press Enter when finished
6. **Win**: Control 60% of the map, eliminate your opponent, or force them into a position with no valid moves

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

### Core Gameplay
✅ Strategic territory expansion (must place adjacent to your territory)
✅ Clean, colorful tile-based graphics with hover effects
✅ Smooth battle animations with visual feedback
✅ Chain reaction battles across the map
✅ Real-time territory percentage tracking
✅ Multiple win conditions (60% control, elimination, or no valid moves)

### User Experience
✅ Intelligent error messages and notifications
✅ Visual feedback for all actions
✅ Hover highlighting for valid placements
✅ Disabled state styling for buttons
✅ Animated modal transitions
✅ Confirmation dialogs for important actions
✅ Mobile-responsive canvas (adapts to screen size)

### Controls & Shortcuts
✅ Undo last move (Ctrl+Z during your turn)
✅ Keyboard shortcuts (1/2/3 for units, Enter to end turn)
✅ Restart game anytime (with confirmation)
✅ Settings persist during gameplay

### AI Opponent
✅ Three difficulty levels with smart decision-making
✅ Three distinct strategies (Defensive, Balanced, Aggressive)
✅ Handles edge cases (no valid moves, elimination)
✅ Strategic unit selection based on enemy composition

## 🎓 Strategy Tips

1. **Counter Your Opponent**: Watch what units the AI uses and place counters
2. **Protect Borders**: Defend tiles adjacent to enemy territory
3. **Chain Reactions**: A well-placed unit can trigger multiple battles
4. **Expand Wisely**: Don't spread too thin - consolidate territory
5. **Use All Units**: Each turn you can place up to 3 units - use them!

## 🛠️ Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Rendering**: HTML5 Canvas with efficient redrawing
- **Styling**: Tailwind CSS (CDN)
- **File Size**: Single HTML file (~25KB)
- **Performance**: 60fps smooth animations
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **Responsive**: Canvas scales to screen size
- **Error Handling**: Comprehensive validation and user feedback

## ✨ Production-Ready Features

This project has been thoroughly reviewed and includes:

### Bug Fixes & Improvements
- ✅ **Fixed critical placement bug**: Players must now place units adjacent to their territory (not anywhere on the map)
- ✅ **Proper AI validation**: AI uses the same placement rules as the player
- ✅ **No-moves detection**: Game properly detects when a player has no valid moves and declares the winner
- ✅ **Hover state management**: Hover effects properly clear when mouse leaves canvas
- ✅ **Disabled button styling**: Buttons visually indicate when they're disabled
- ✅ **Modal animations**: Smooth fade-in effects for game over screen
- ✅ **Restart confirmation**: Prevents accidental game restarts

### User Experience Enhancements
- ✅ **Visual notifications**: Toast-style notifications for all actions (success, warning, error, info)
- ✅ **Shake animations**: Invalid actions trigger visual feedback
- ✅ **Error messages**: Clear, helpful messages for invalid actions
- ✅ **Success feedback**: Confirmation when units are placed successfully
- ✅ **Keyboard shortcuts**: Fast gameplay with 1/2/3, Enter, and Ctrl+Z
- ✅ **Better win/loss messages**: Shows why the game ended (elimination, percentage, no moves)

### Code Quality
- ✅ **Proper validation**: All user inputs validated before processing
- ✅ **Edge case handling**: No-moves, elimination, chain reactions all handled correctly
- ✅ **Consistent styling**: Disabled states, hover effects, animations all polished
- ✅ **Mobile responsive**: Canvas adapts to different screen sizes
- ✅ **Clean code structure**: Well-organized methods with clear responsibilities

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

### Mouse Controls
- **Select Unit**: Click unit buttons on left panel
- **Place Unit**: Click on valid tiles (adjacent to your territory, highlighted on hover)
- **End Turn**: Click "End Turn" button
- **Undo**: Click "Undo Move" (only during your turn, Ctrl+Z)
- **Restart**: Click "Restart Game" (confirms if game in progress)
- **Settings**: Change map size, AI difficulty, and strategy

### Keyboard Shortcuts
- **1**: Select Warrior
- **2**: Select Archer
- **3**: Select Mage
- **Enter**: End turn (if units placed)
- **Ctrl+Z / Cmd+Z**: Undo last move

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

## 💡 Future Enhancements (Optional)

These features could be added but are not critical for a great experience:

- 🔊 Sound effects for battles and actions
- 💾 Save/load game state (localStorage)
- 🎵 Background music toggle
- 🏆 Score tracking across multiple games
- 📱 Enhanced mobile touch controls (currently works but optimized for desktop)
- 👥 Local multiplayer mode (pass-and-play)
- 🎨 Theme customization options
- 📊 Statistics and analytics dashboard
- 🏅 Achievement system

## 📜 License

Free to use and modify. Created as a strategy game demo.

## 🎉 Enjoy!

Have fun conquering territory and outsmarting the AI! Try different strategies and difficulty levels to master the game.
