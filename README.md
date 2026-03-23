# Maze

## Project Overview
This project implements a console-based maze game written in C.

Players navigate through a maze from the starting point (P) to the exit (E) within a limited number of steps.  
During exploration, players encounter different events and mini-games that affect the remaining steps and final outcome.

The project emphasizes real-time interaction, game logic design, and modular function organization.

## Game Features

### Maze System
- Player movement using arrow keys
- Step-limited gameplay
- Hidden paths and breakable walls
- Real-time console rendering

### Event System
|     Symbol     |             Description            |
|----------------|------------------------------------|
|        ?       |         Optional challenge         |
|        !       |          Forced mini-game          |
|        *       |     Special challenge (Sudoku)     |


## Mini Games

### Typing Game
- Type falling characters correctly
- Score determines step reward

### Memory Matching
- Match pairs in a 6x6 grid
- Based on memory and speed

### Counting Game
- Track objects entering and leaving
- Answer logic-based questions

### Spelling Game
- Observe falling letters
- Reconstruct correct English words

### Sudoku Challenge
- Solve a Sudoku puzzle
- Earn special rewards

## Difficulty Modes
Players can select different difficulty settings at the start:

1. More steps + easier mini-games  
2. More steps only  
3. Easier mini-games only  
4. Original mode  

## Achievement System
The game includes multiple achievements, such as:
- Game completion
- Hidden path discovery
- Retry ability
- No-penalty protection
- Playing all mini-games

Achievements contribute to the final score.

## Scoring System
Final score is calculated based on:
- Remaining steps
- Mini-game performance
- Achievements unlocked

## Technical Details
- Language: C
- Platform: Windows Console

### Key Techniques
- Real-time input handling (`getch`, `kbhit`)
- Console cursor control (`gotoxy`)
- Random event generation (`rand`)
- State management (steps, achievements, buffs)

## Project Structure
- main.c            : Main game loop and system integration
- maze.txt          : Maze layout data
- sudoku.txt        : Sudoku puzzle data
- utilwin32.h       : Console utility functions

## How to Run (Windows GCC)

1. Compile:
   gcc main.c -o maze.exe

2. Run:
   maze.exe

Make sure `maze.txt` and `sudoku.txt` are in the same directory.

## Design Note
This project is implemented in a single source file, but follows a modular design.  
Different systems (maze, event handling, mini-games) are separated into functions for clarity and maintainability.

## Author
Yi-An, Yang

## Acknowledgements
- Console utility functions (`utilwin32.h`) are adapted from publicly available Windows API examples.
- Some resource files (maze and Sudoku data) are text-based assets.
## Acknowledgements
- Console utility functions (`utilwin32.h`) are adapted from publicly available Windows API examples.
- Some resource files (maze and Sudoku data) are text-based assets.
