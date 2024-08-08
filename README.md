# Tic-Tac-Toe Game

This project is a simple command-line implementation of the classic Tic-Tac-Toe game in Python. It allows a human player to play against a computer opponent with random moves.

## Features

- **Human vs. Computer**: Play against a computer that makes random moves.
- **Command-line Interface**: Simple and easy-to-use text-based interface.
- **Dynamic Game Board**: The game board is updated after each move and displayed to the player.
- **Win Detection**: The game automatically detects if a player has won or if the game is a tie.

## Project Structure

- **`tictactoe.py`**: Main game logic, including the game loop, board display, move validation, and winner detection.
- **`player.py`**: Defines the `Player` classes for both human and computer players.

## Requirements

- Python 3.x

## How to Play

1. Clone the repository or download the code.
2. Navigate to the directory containing the code.
3. Run the game using Python:

   ```sh
   python tictactoe.py
   ```

4. Follow the on-screen instructions to input your move.

## Classes

### TicTacToe

- **`__init__(self)`**: Initializes the game board and winner.
- **`print_board(self)`**: Prints the current state of the game board.
- **`print_board_nums()`**: Prints the board numbers to indicate positions (0-8).
- **`available_moves(self)`**: Returns a list of available moves.
- **`empty_squares(self)`**: Returns `True` if there are empty squares.
- **`num_empty_squares(self)`**: Returns the number of empty squares.
- **`make_move(self, square, letter)`**: Places a letter on the board if the move is valid.
- **`check_winner(self, square, letter)`**: Checks if the current move results in a win.

### Player (in `player.py`)

- **Player**: Base class for players.
- **RandomComputerPlayer**: Subclass of `Player` that makes random moves.
- **HumanPlayer**: Subclass of `Player` that takes input from the user for their move.

## Gameplay Flow

1. **Initialization**: The game initializes a 3x3 board.
2. **Player Move**: The human player is prompted to enter a move.
3. **Computer Move**: The computer makes a random move.
4. **Board Update**: After each move, the board is updated and displayed.
5. **Win/Tie Check**: The game checks for a winner or a tie after each move.
6. **Game End**: The game announces the winner or declares a tie.

## Future Improvements

- Implement a smarter AI for the computer player.
- Add a graphical user interface (GUI) for easier play.
- Include options for a two-player mode.
- Improve error handling and input validation.

## License

This project is open-source and free to use. Feel free to modify and share!

Enjoy playing Tic-Tac-Toe!