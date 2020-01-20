# guess-guess-who

Is there a better way to play "Guess Who?". A cursory investigation. 

The results of this project are hosted on https://tychenne.github.io/guess-guess-who/

This project is based on the paper published by [Mihai Nica called "Optimal Strategy in "Guess Who?": Beyond Binary Search](https://arxiv.org/abs/1509.03327). From the abstract, 
> "Guess Who?" is a popular two player game where players ask "Yes"/"No" questions to search for their opponent's secret identity from a pool of possible candidates. This is modeled as a simple stochastic game. Using this model, the optimal strategy is explicitly found. Contrary to popular belief, performing a binary search is _not_ always optimal. Instead, the optimal strategy for the player who trails is to make certain bold plays in an attempt catch up. This is discovered by first analyzing a continuous version of the game where players play indefinitely and the winner is never decided after finitely many rounds. 

In this project, I replicate the study by running the algorithm on various <n, m, P1> starting positions, n being the candidate pool open to player 1 (_n_ which includes the opponent's secret identity), m being the candidate pool open to player 2, and P1 telling us it is player 1's turn. At the end, I compare player 1's win rate that is (number of wins/number of games) for each of the <n, m, P1> starting positions with their corresponding theoretical lower bound win rate whose formula is derived in the paper. 
