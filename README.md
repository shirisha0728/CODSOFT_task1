# CODSOFT_task1
## TIC TAC TOE AI
Tic Tac Toe, also known as Noughts and Crosses, is a classic two-player game. The game is played on a 3x3 grid, where players take turns marking a space with either an “X” or an “O”. The objective is to be the first to get three of your marks in a row, either horizontally, vertically, or diagonally.
# Overview
The code implements a Tic Tac Toe game where a player competes against a computer. The computer uses the Minimax algorithm to make optimal moves.

## Key Components
1. Board Representation:
 The board is represented as a dictionary with keys from 1 to 9, each corresponding to a position on the Tic Tac Toe grid.
2. Functions:
  * printBoard(board): Prints the current state of the board.
  * spaceIsFree(position): Checks if a given position on the board is free.
  * insertLetter(letter, position): Inserts a letter (‘X’ or ‘O’) at the specified position and checks for a win or draw.
  *  checkWin(): Checks if there is a winning combination on the board.
  * checkWhichMarkWon(mark): Checks if a specific mark (‘X’ or ‘O’) has won.
  *  checkDraw(): Checks if the game is a draw.
  *  playerMove(): Prompts the player to enter a position and makes the move.
  *  compMove(): Determines the best move for the computer using the Minimax algorithm and makes the move.
  * minimax(board, isMaximizing): Implements the Minimax algorithm to evaluate the best possible move for the computer.
3. Game Flow
   * Initialization: The board is initialized with empty spaces, and the player and computer are assigned ‘O’ and ‘X’, respectively.
   * Player Move: The player is prompted to enter a position, and the move is made.
   * Computer Move: The computer calculates the best move using the Minimax algorithm and makes the move.
   * Win/Draw Check: After each move, the game checks for a win or draw. If either condition is met, the game ends with an appropriate message.
   * Loop: The game continues in a loop until there is a win or a draw.
## MINIMAX Algorithm
The Minimax algorithm is a popular choice for creating an unbeatable Tic Tac Toe game. Here’s a brief overview of how it works:

# Minimax Algorithm Overview
* Objective: The algorithm aims to minimize the possible loss for a worst-case scenario. It assumes that the opponent is also playing optimally.
* Scoring:
  * Win: +10 points
  * Loss: -10 points
  * Draw: 0 points
* Process:
* Recursion: The algorithm recursively explores all possible moves.
* Evaluation: It evaluates the board state after each move.
* Maximizing and Minimizing:
When it’s the AI’s turn, it chooses the move with the maximum score.
When it’s the opponent’s turn, it chooses the move with the minimum score.