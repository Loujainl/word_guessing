# word_guessing
Tiime algorithm test
A word game 
- Alice chooses a 10-letter word from a fixed dictionary
- Bob proposes a word from the same dictionary
- For each proposal, Alice returns the "score" of the proposed word:
  * each correct letter gives 1 point,
  * plus an additional point if it is at the right position.
  * The total score of Bob is the sum of scores over k rounds with k fixed to 5, 10 or 15.
- The goal is to maximize the score of Bob over 100 games
  
- Precomputation (less than one hour)
 * Less than one second in my solution
- and your code should play any game in a reasonable amount of time (less than a few minutes)
 * One minute in my solution.

- Typical good scores we expect are for instance: 30 (k=5), 60 (k=10), 74 (k=15).
 * Results achieved in 1 minute
