
## A word guessing game inspired by the French TV show "Motus". - Tiime algorithm test

## Table of Contents
1. [Problem Definition](#problem-definition)
2. [Heuristic Greedy Strategy](#heuristic-greedy-strategy)
3. [Results](#results)


### Problem Definition
In this game:
- Alice selects a 10-letter word from a dictionary.
- Bob tries to guess the word by proposing words from the same dictionary.
- Scoring:
  - +1 point for each correct letter.
  - +2 points if the letter is in the correct position.
- Bob aims to maximize his score over 100 games, each played over 5, 10, or 15 rounds.


### Heuristic Greedy Strategy
1. **Precompute Letter Frequencies**: Calculate the frequency of each letter in the entire dictionary.
2. **Precompute Bi-gram Frequencies**: For each letter, calculate the frequency of the letters that follow it.
3. **Precompute Positional Letter Frequencies**: Calculate the frequency of each letter at each specific position in the word.
4. **Compute a Grade for Each Word**: Evaluate each word in the dictionary according to frequency metrics and assign a grade.
5. **Greedy First Guess**: Choose from candidate words with the maximum grade.
6. **Use the Clue Signal for Informed Guesses**: Filter candidate words to ensure only words with matching scores remain.

### Results
- **k = 5**: Score 32.08
- **k = 10**: Score 61.34
- **k = 15**: Score 75.83
- **Runtime**: Precomputation: 0.31 seconds, 100 games: 1 minute

