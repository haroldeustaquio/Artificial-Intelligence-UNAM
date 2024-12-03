# Repository of Algorithmic Games and Decision Making

## Overview

This repository brings together practical examples of search and decision-making algorithms in the context of artificial intelligence applied to games. Through these algorithms, fundamental concepts in strategic decision making are explored, both in adversarial games and in environments with real-time decision making.

**Content**

- [Implemented Algorithms](#implemented-algorithms)
    - [Adversarial Search Algorithms](#adversarial-search-algorithms)
    - [Real-Time Decision Making](#real-time-decision-making)
    - [Games of Possibility and Strategies under Uncertainty](#games-of-possibility-and-strategies-under-uncertainty)
- [Games in the Repository](#games-in-the-repository)

---

## Implemented Algorithms

### Adversarial Search Algorithms

In games where two or more players compete directly (adversarial games), the strategy is focused on maximizing one's own gain and minimizing the opponent's. Search algorithms such as Minimax and Alpha-Beta pruning are essential in these contexts:

- **Minimax**: This algorithm generates a decision tree of all possible moves, simulating player and opponent turns. At each node, the move that maximizes the player's score or minimizes the opponent's is chosen, which allows anticipating and countering the opponent's actions.

- **Alpha-Beta Pruning**: This is an optimization of the Minimax algorithm that reduces the number of nodes evaluated. By introducing alpha (best guaranteed outcome for the player) and beta (best outcome for the opponent) values, the algorithm ignores unnecessary branches of the tree, speeding up the search without losing accuracy in choosing the best move.

Application example: These algorithms are ideal for zero-sum games, such as chess and Tic-Tac-Toe, where the goal is to maximize one's own options while minimizing those of the opponent.

### Real-Time Decision Making

In real-time environments, decisions must be made quickly without full analysis, a common challenge in strategy video games or robotics. Approaches to addressing real-time decision making include:

- **Search depth reduction**: Limiting the search in the decision tree to only evaluate the most likely moves instead of analyzing every possibility, allowing for a faster response.

- **Heuristic Functions**: Using a heuristic function to quickly assess the quality of a position without having to explore all possible continuations, thus allowing for an efficient response in high-pressure environments.

Application example: This type of decision making is used in games such as Space Invaders, where the player or AI system needs to react to events in real time.

### Games of Possibility and Strategies under Uncertainty

In games where chance is a determining factor and there is uncertainty in the results (chance games), algorithms must make decisions considering uncertain conditions. In these cases, common strategies include:

- **Probabilistic Evaluation**: Possible outcomes of plays are estimated taking into account probabilities and the lack of complete information, which allows uncertainty to be managed in risky decisions.

Application example: This approach is common in games such as Craps, where the strategy must consider the chance inherent in the game and the probability of each outcome.

---
## Games in the Repository

This repository contains implementations of the following games, each designed to exemplify one or more of the concepts of search and decision-making algorithms:

- **Nim**
- **Tic-Tac-Toe**
- **Space Invaders**
- **Time Reaction**
- **Craps**

---

<div align="center"> 
  <em> 
    We believe in the power of collaboration. If you have ideas, suggestions, or improvements, feel free to open an issue or submit a pull request. Let’s make this project even better—your contributions are always welcome! 
  </em> 
</div>