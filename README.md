# Python Rush 🐍.

A modern twist on the classic Snake game with programming-themed elements, portals, and dynamic challenges.

![Game Screenshot](https://via.placeholder.com/500x300/121214/FFFFFF?text=Python+Rush+Gameplay)

## 🎮 Features

### Core Gameplay
- **Classic Snake Mechanics** with a programming twist
- **Fill the entire grid** to win the game
- **Three difficulty levels**:
  - Junior (30×30 grid) - Easy
  - Midl (75×75 grid) - Medium
  - Sinior (90×90 grid) - Hard

### Programming-Themed Elements
- **Python codes `</>`** - Collect for +1 point
- **C++ codes `c++`** - Avoid! Lose -5 points and 2 snake segments
- **Dynamic scoring system** with visual feedback

### Advanced Mechanics
- **Portals System**:
  - Blue and orange connected portals
  - 60-second lifetime with countdown timer
  - Smart teleportation avoiding obstacles
  - Cooldown system to prevent rapid teleportation
- **Speed Boost** - Hold Shift to double movement speed
- **Pulse animations** and glowing effects
- **Sound effects** for all interactions

## 🎯 How to Play

### Objective
Fill every cell on the grid with your snake to win! Collect Python codes, avoid C++ codes, and use portals strategically.

### Controls
- **W/↑, A/←, S/↓, D/→** - Move the snake
- **Shift** - Hold to double movement speed
- **Space** - Pause/resume game
- **Mouse** - Click UI buttons for game control

### Game Rules
1. **Start** - Click "Играть" (Play) to begin
2. **Difficulty** - Select from dropdown before starting
3. **Scoring**:
   - Python code `</>`: +1 point
   - C++ code `c++`: -5 points and lose 2 segments
4. **Portals** - Enter one portal to exit through the other
5. **Game Over** conditions:
   - Hit the wall
   - Collide with yourself
   - Run out of space

## 🚀 Installation & Running

### Prerequisites
- Python 3.7+
- PyGame library

### Quick Start
```bash
# Clone the repository
git clone https://github.com/yourusername/python-rush.git
cd python-rush

# Install dependencies
pip install pygame numpy

# Run the game
python python_rush_final.py
```

### Alternative: No NumPy
If NumPy installation fails, the game will still run with basic sound functionality.

## 🖥️ System Requirements

### Minimum
- **OS**: Windows 7+, macOS 10.12+, or modern Linux
- **Resolution**: 1024×768 minimum
- **Memory**: 512MB RAM
- **Storage**: 50MB free space

### Recommended
- **Resolution**: 1280×720 or higher
- **Memory**: 1GB RAM
- **Sound**: Audio output for full experience

## ⚠️ Known Issues & Compatibility

### Display Issues
The game **may not display correctly** on:
- **Ultra-narrow monitors** (width < 1024px)
- **Small screens** (diagonal < 12")
- **Non-standard aspect ratios** (4:3 or 16:10 recommended)

### Workarounds
1. **Windowed mode**: Run on lower resolution if fullscreen has issues
2. **Scale down**: Modify `WINDOW_SIZE` in code for smaller displays
3. **Font issues**: Game uses Consolas font - fallbacks available

### Audio Issues
If you encounter sound problems:
- Game will run silently without PyGame audio support
- No NumPy required for core gameplay
- Sound is optional enhancement

## 🎨 Technical Highlights

### Code Architecture
- **Modular design** with separate functions for game logic, rendering, and sound
- **Event-driven** PyGame loop optimized for 60 FPS
- **State management** for game flow (running, paused, game over)

### Visual Features
- **Dynamic grid scaling** for different difficulty levels
- **Glowing effects** using layered alpha surfaces
- **Pulse animations** on portals
- **Clean UI** with consistent theming

### Sound System
- **Procedural audio generation** for platform compatibility
- **Four distinct sound effects**:
  - High beep (collecting Python code)
  - Low beep (collecting C++ code)
  - Mid-tone (teleportation)
  - Deep tone (game over)

## 📊 Game Statistics

| Metric | Junior | Midl | Sinior |
|--------|--------|------|--------|
| Grid Size | 30×30 | 75×75 | 90×90 |
| Cells | 900 | 5,625 | 8,100 |
| Base Speed | 10 moves/sec | 10 moves/sec | 10 moves/sec |
| Boost Speed | 20 moves/sec | 20 moves/sec | 20 moves/sec |
| Portal Cooldown | 60 sec | 60 sec | 60 sec |

## 🔧 Customization

You can modify these constants in the code:

```python
# In python_rush_final.py
WINDOW_SIZE = 500          # Change for different resolutions
MOVES_PER_SECOND = 10      # Adjust base speed
PORTAL_LIFETIME_MS = 60000 # Change portal duration
MAX_ITEMS = 10             # Maximum items on screen
```

## 🐛 Troubleshooting

### Common Issues
1. **Game won't start**: Ensure PyGame is installed: `pip install pygame`
2. **No sound**: Install NumPy or accept silent mode
3. **Small window**: Edit `WINDOW_SIZE` variable
4. **Control lag**: Check FPS counter, reduce background processes

### Error Messages
- `pygame.error: Unable to open a audio device` → Run without sound
- `ModuleNotFoundError: No module named 'numpy'` → Game runs with basic audio
- `Display mode not supported` → Reduce `WINDOW_SIZE` value

## 🤝 Contributing

Contributions welcome! Areas for improvement:
- Additional power-ups
- More programming language themes
- High score tracking
- Level progression system
- Mobile compatibility

### Development Setup
```bash
# Fork and clone
git clone https://github.com/yourusername/python-rush.git

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dev dependencies
pip install -r requirements.txt
```

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **PyGame community** for excellent documentation
- **Python Software Foundation** for the inspiration
- **Classic Snake games** that inspired this modern take
- **Open source contributors** to all libraries used

## 🎉 Enjoy Playing!

Experience the thrill of programming-themed snake action. Can you fill the entire grid and become the ultimate Python Rush champion?

---

*Note: Game interface is in Russian but intuitive for all players. "Играть" = Play, "Сложность" = Difficulty, "Стоп" = Stop/Pause.*
