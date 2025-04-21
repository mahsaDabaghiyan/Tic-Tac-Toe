# Tic Tac Toe GUI - Python Tkinter

A graphical Tic Tac Toe game built with Python using Tkinter. 
The board size is customizable (e.g., 3×3, 4×4, etc.), and the game supports two-player mode with X and O.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Function Descriptions](#function-descriptions)
- [How to Play](#how-to-play)
- [Run & Usage](#run--usage)
- [Author](#author)

---

## Project Overview

This project is a Tic Tac Toe game implemented in Python using the Tkinter GUI library. 
Users can enter the desired board size (e.g., 3 for 3×3, 4 for 4×4) to start the game. 
Players take turns clicking on empty cells to place their mark (X or O), and the game checks for a winner after each move. 
If a player wins or the board is full (tie), a message is shown and the board resets automatically.

---

## Function Descriptions

### `__init__(self, board_size=3)`
- Initializes the game window, board matrix, current player, and GUI buttons.

### `create_board_buttons(self)`
- Creates a grid of buttons in the GUI representing the game board.

### `make_move(self, row, col)`
- Called when a player clicks on a cell: 
  Places the current player's mark, checks for a win/tie, switches players, or shows an error if the move is invalid.

### `check_win(self, player)`
- Checks all rows, columns, and diagonals to determine if the player has won.

### `is_full(self)`
- Determines if the board is completely filled, indicating a tie.

### `reset_game(self)`
- Resets the board and GUI buttons to start a new game.

### `run(self)`
- Starts the Tkinter main loop to run the game window.

---

## How to Play

1. Run the program and enter your desired board size (e.g., `3` for a 3×3 game).
2. Two players take turns: Player X starts, followed by Player O.
3. Click an empty cell to place your mark.
4. The first player to align all their marks in a row, column, or diagonal wins.
5. If all cells are filled and there is no winner, the game ends in a tie.
6. The game resets automatically after a win or tie for continuous play.

---

## Run & Usage

### Requirements:
- Python 3.x
- Tkinter (included by default with most Python installations)

### Run the game:
```bash
python tic_tac_toe_gui.py
