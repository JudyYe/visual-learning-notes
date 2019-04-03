# Deep RL

## intro
- some consequences of action is lifelong
    + to live a good life, robot should make good decisions
    + reward can be short / long term

# MDP __Markov Decision Processes__
- fundamental framework for RL 
- stochastics model
    + finite set of states S
    + finite set of actions A*
    + immediate reward function R: $S \times A -> Reals$
    + Transition function $T$: $S\times A -> S$
- policy
    + $\pi: S->A$ state into actions
- Value
    +  mapping staes to real number
    +  for any policy $\pi$, define the (expected) return to be the function V: S->Reals
    +  optimal value: larger than any policy and any state
-  how to find optimal policy?
    +  brute force
    +  dynamic Proramming 
        *  __Bellman Equation__ 
        *  recursive way of understanding  value
    + how to solve Bellman equations
        * value iteration method
        * policy iteration method
- Q value
    + state AND ACTION
        * $Q^\pi (s, a ) = \sum_{i = 0}^\inft \gamma r(t)$

# Modern view
- reward / state / transition function are no longer known
- estimate by experimenting them
- we don't need to search over all state space.
