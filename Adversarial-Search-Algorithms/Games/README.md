# Games

In the field of artificial intelligence and game theory, games are considered a form of interaction between two or more agents (players) who seek to maximize their gains or minimize their losses in a competitive environment. Games can be classified into several categories, with the most relevant being:

1. **Zero-Sum Games**: In these games, one player's gains are exactly equal to the losses of another player. A classic example is chess.

2. **Deterministic Games**: These games have a predictable outcome based on the players' decisions. There are no elements of chance involved.

3. **Simultaneous and Sequential Games**: In simultaneous games, players make decisions at the same time without knowing the other's choices. In sequential games, players take turns.

Search algorithms in games focus on finding the best possible move by exploring the possible game configurations and evaluating the outcome of each.

---

## Implementation

### 1. Tic-Tac-Toe

**Description**: This is a two-player game played on a 3x3 board. Players place their marks (X or O) in an attempt to align three of their marks in a row, column, or diagonal.

**Simplified Implementation**:
- **Board**: An empty board is created, represented as a list of lists.
- **Turns**: Players take turns entering the coordinates (row and column) where they want to place their mark.
- **Winner Verification**: After each move, it checks if any player has managed to align three marks (horizontal, vertical, or diagonal). If a player wins, the game ends. If the board is full without a winner, it declares a tie.

### 2. Nim

**Description**: In this game, there are several piles of sticks, and players alternate turns to remove sticks from a pile. The objective is to force the opponent to be the one who cannot make a move.

**Simplified Implementation**:
- **Piles**: Several piles of sticks are initialized with different quantities.
- **Turns**: Players choose a pile and decide how many sticks to remove (at least one, but not more than the amount in the chosen pile).
- **End of the Game**: The game continues until there are no sticks left in any pile. The player who cannot make a move (because all piles are empty) loses.

---

## Conclusion

Both games are classic examples that illustrate important concepts in game theory and search algorithms. Implementing these games in Python allows for a practical understanding of how turns, victory condition verification, and strategic decision-making work. These principles can be extended to more complex games and the creation of agents that play effectively.