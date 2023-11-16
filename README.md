# Book-recommendation-system
A project for creating a book recommendation system using reinforcement learning and other AI techniques with book review data.

## Objectives of recommendation system
We want to recommend particular books to users based on a number of factors which could include some of the following non-exhaustive list:
 - reading history (books & their ratings given by user)
 - favoured publishers
 - favoured authors
 - popular books of similar genre

I plan to use RL techniques to create this recommendation system and thus we can model the problem as a Markov decision process (MDP). The following elements make up the MDP:
 - X_t is the current state and represents the history of books read/reviewed by the user
 - S is the state space and contains all possible values of X_t, S = {all subsets of the total set of all considered books in the model}
 - Y_t is the current action and represents the next recommendation to be made
 - the action space, A, is the set of all books being considered in the model
 - admissable actions, A(s) = A\s
 - the rewards are some function of: the review given by the user of the recommended book, the completion of the recommended book and the initial interest in the book (if the user started the read at all)
