# Pooja Makwana-202404020
# Jainil Sutariya-202404042
# Snake Game (C++ Console Version)

## Overview
This is a simple **Snake Game** implemented in **C++** using a **linked list** for dynamic snake growth. The game runs in the **Windows Console**, using the Windows API for smooth rendering. The snake moves automatically, and the player controls the direction using keyboard inputs. The goal is to eat fruits (`*`), grow in length, and achieve the highest score.

## Features
- **Dynamic Snake Growth**: Uses a linked list structure to grow the snake dynamically.
- **Smooth Console Rendering**: Uses **Windows API (HANDLE, CHAR_INFO)** for efficient game rendering.
- **Collision Detection**:
  - Wall collision (`#` border) ends the game.
  - Self-collision (snake biting itself) ends the game.
- **Random Fruit Placement**: Fruits spawn in random positions, ensuring they don't overlap with the snake.
- **Speed Adjustment**: The snake speeds up as it eats more fruit (`frameDelay` decreases).
- **Pause & Resume**: Press **'P'** to pause or resume the game.
- **High Score Tracking**: Tracks the highest score across multiple runs.
- **Game Countdown Timer**: Before the game starts, a countdown appears for better user experience.
- **Play Again Option**: After a game ends, the player can choose to restart or exit.

## Controls
- **W** - Move Up
- **A** - Move Left
- **S** - Move Down
- **D** - Move Right
- **P** - Pause/Resume

## How to Run
### Prerequisites
- **Windows OS** (Uses Windows-specific APIs like `windows.h`, so it won't work on Linux/Mac without modifications.)
- **C++ Compiler (MinGW or MSVC)**

### Compilation & Execution
1. **Compile using g++ (MinGW or MSVC):**
   ```sh
   g++ snake_game.cpp -o snake_game.exe
   ```
2. **Run the executable:**
   ```sh
   snake_game.exe
   ```

## Game Rules
1. The snake moves automatically in the last chosen direction.
2. Eating a fruit (`*`) increases the snake's length and score.
3. If the snake hits the wall or itself, the game ends.
4. The game gets faster as you eat more fruits.
5. If you reach **15 fruits**, you win!
6. The game displays the **current score** and the **high score**.

## Known Limitations
- The game runs only on **Windows** (due to the `windows.h` dependency).
- Console resizing may cause unexpected behavior.
- No graphical interface (pure text-based game).

## Future Improvements
- Porting to **Linux/Mac** (replacing `windows.h` with cross-platform libraries like `ncurses`).
- Adding **sound effects** and **background music**.
- Implementing **multiplayer mode** or AI-driven obstacles.

## Credits
Developed by: **[Your Name]**  
Language: **C++**  
Platform: **Windows Console**

Enjoy the game! 🎮🐍

