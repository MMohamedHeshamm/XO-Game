# Tic-Tac-Toe (XO Game) — C++

![Language](https://img.shields.io/badge/Language-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![Interface](https://img.shields.io/badge/Interface-Console-555555)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D4?logo=windows&logoColor=white)

A two-player **Tic-Tac-Toe (XO)** game written in **C++** and played directly in the Windows console. This project practices fundamental programming concepts such as 2D arrays, control flow, functions, user input validation, and game-state management.

## Features

- **Local two-player gameplay:** Player 1 uses `X`, and Player 2 uses `O`.
- **Numbered 3×3 board:** Players select a position from `1` to `9`.
- **Move validation:** Rejects out-of-range input and already occupied cells.
- **Win detection:** Checks rows, columns, and diagonals.
- **Draw detection:** Recognizes a full board without a winner.
- **Play again:** Lets players start another round after a game ends.

## How to Play

At the start of a round, the board positions are numbered:

```text
  1 | 2 | 3
 ---+---+---
  4 | 5 | 6
 ---+---+---
  7 | 8 | 9
```

1. Run the program in a console.
2. Player 1 (`X`) enters a number between `1` and `9`.
3. Player 2 (`O`) chooses an available position.
4. Take turns until a player makes three symbols in a row or the board fills up.
5. When prompted, enter `Y` to play another round, or any other character to exit.

## Getting Started

### Prerequisites

- A **C++ compiler** such as GCC (MinGW-w64) or the compiler included with Code::Blocks.
- **Windows**, as the current implementation uses `system("cls")` to clear the console.

### Build and Run (G++)

Clone the repository:

```bash
git clone https://github.com/MMohamedHeshamm/XO-Game.git
cd XO-Game
```

Compile the source file:

```bash
g++ main.cpp -o XO-Game.exe
```

Run it in Windows PowerShell:

```powershell
.\XO-Game.exe
```

Alternatively, open the provided `x o new.cbp` project in **Code::Blocks** and use **Build and Run** with a configured C++ compiler.

## Project Structure

```text
XO-Game/
├── main.cpp            # Game board, player turns, validation, win/draw logic
├── x o new.cbp          # Code::Blocks project configuration
└── README.md            # Project documentation
```

> The repository currently also contains IDE-generated and build-output files. These are not required to understand the game logic and can be excluded from version control.

## Programming Concepts Demonstrated

- **Two-dimensional arrays** to represent the game board.
- **Functions** to display the board and manage the game.
- **Loops and conditional statements** to control turns and game rules.
- **Switch statements** to map user choices to board cells.
- **Input validation** to handle invalid and occupied positions.

## Notes and Future Improvements

This is a small, beginner-friendly C++ project focused on programming fundamentals, not a graphical game or an AI opponent.

Potential improvements include:

- Refactoring repeated move-handling and win-checking code into reusable functions.
- Making console clearing cross-platform.
- Adding an optional single-player mode against the computer.
- Adding automated tests for win, draw, and invalid-move scenarios.

## Author

**Mohamed H. Eldesouky**  
GitHub: [@MMohamedHeshamm](https://github.com/MMohamedHeshamm)
