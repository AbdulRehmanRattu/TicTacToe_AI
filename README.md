
# Tic-Tac-Toe Game with AI Opponent

This project implements a Tic-Tac-Toe game in Python, featuring an AI opponent powered by the Minimax algorithm. The game includes a graphical user interface (GUI) built using the Pygame library, allowing players to challenge an optimally playing AI.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Game Mechanics](#game-mechanics)
- [AI Implementation](#ai-implementation)
- [Testing and Results](#testing-and-results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview
The Tic-Tac-Toe game is a classic two-player game where players take turns marking spaces in a 3x3 grid with X or O. The goal is to place three of your marks in a horizontal, vertical, or diagonal row before your opponent. This project enhances the traditional game by introducing an AI opponent that uses the Minimax algorithm to play optimally.

## Features
- Simple and intuitive GUI using Pygame
- Play against an AI opponent using the Minimax algorithm
- AI ensures at least a draw with optimal play
- Detailed game state management and analysis
- Performance testing and outcome reporting

## Installation
To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/tictactoe-ai.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd tictactoe-ai
   ```

3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To start the game, run the following command:
```bash
python tictactoe.py
```
The GUI will launch, and you can start playing by clicking on the grid to place your mark.

## Game Mechanics
The game consists of several key functions to manage the game state:

- **initial_state**: Initializes the game board as a 3x3 grid of `None` values.
- **player**: Determines the current player's turn based on the count of X and O on the board.
- **actions**: Returns all possible moves available on the board as tuples (i, j).
- **result**: Calculates the board state resulting from a player's move, ensuring validity.
- **winner**: Checks for a winning condition by evaluating rows, columns, and diagonals.
- **terminal**: Determines if the game has ended by win or draw.
- **utility**: Assigns a numerical value to the game's end state: 1 for a win by X, -1 for a win by O, and 0 for a draw.

## AI Implementation
The core of the AI is the Minimax algorithm, which evaluates all possible future game states and selects the move that maximizes the AI's chance of winning while minimizing the opponent's chance. The algorithm ensures that the AI can secure a draw at minimum when playing optimally.

## Testing and Results
The AI was tested in a series of ten games, with the following outcomes:

- **User as X**:
  - Total Games: 6
  - Wins: 0
  - Ties: 6
  - Losses: 0

- **User as O**:
  - Total Games: 4
  - Wins: 0
  - Ties: 2
  - Losses: 2

The results demonstrate the effectiveness of the Minimax algorithm in ensuring a draw or better when the AI plays optimally.

## Contributing
Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are gladly accepted.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Contact
For any questions or inquiries, please contact:

- **Email**: rattu786.ar@gmail.com
- **LinkedIn**: [Abdul Rehman Rattu](https://www.linkedin.com/in/abdul-rehman-rattu-395bba237)

---

Thank you for using this Tic-Tac-Toe game project! Enjoy playing and exploring the AI opponent.
