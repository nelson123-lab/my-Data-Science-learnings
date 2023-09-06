The difference between first and second order Markov models lies in the level of dependency they consider when predicting future states in a sequence.

In a first order Markov model, the prediction of the next state depends solely on the current state. It assumes that the probability of transitioning to a particular state only depends on the current state and is independent of the previous states. This means that the model only considers the immediate history when making predictions.

On the other hand, a second order Markov model takes into account not only the current state but also the previous state when predicting the next state. It considers the probability of transitioning to a particular state based on the current and previous states. This allows the model to capture more complex patterns and dependencies in the sequence.

To summarize, a first order Markov model considers only the current state, while a second order Markov model considers both the current and previous states when predicting the next state in a sequence. The higher the order of the Markov model, the more historical context it considers, but it also increases the complexity of the model.

We can see how this works in another toy language model for our computer commands. We expect that this one will only ever see two sentences, in a 40/60 proportion.

Check whether the battery ran down please.
Check whether the program ran please.

A Markov chain illustrates a first order model for this.
<p align="center"><img src="image_data in readme/markov_chain_2.png" width="800" height="440"></p>

The first order transition matrics will be as follows:-
<p align="center"><img src="image_data in readme/transition_matrix_first_order_2.png" width="900" height="900"></p>

For the second order the representation will be as follows:-
<p align="center"><img src="image_data in readme/transition_matrix_second_order.png" width="900" height="900"></p>

Notice how the second order matrix has a separate row for every combination of words (most of which are not shown here). That means that if we start with a vocabulary size of N then the transition matrix has N^2 rows.
