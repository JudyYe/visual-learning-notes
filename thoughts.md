# thoughts on stochastic, multimodality, future prediction
`Sept 26`

## When we talk about the stochastic, 
- what do we want to model?
- what can we model?
- How much do the data vary?
- How to test it?


## Formulation 
- encoder should encode all information that gives away the future. -> current frame / state + latent variable --> deterministic.

- two types of stochastic, e.g. HMM
    + transition probability. discrete, diverse, but should be stable over time. once trapped, you should stay with high probability
    + emision probability: gaussian error. Once you are certain state, the gaussian noise should be almost i.i.d for each step.
- **do the analysis still true for natural image prediciton???**
    + transition probability: we do not know in advance how many categories we need.

- reparameterization trick, when should we allow reparameterzation? 
    + reparameterization trick says: how to estimate the gradient of other possible future w.r.t. the reality.
    + transitional stochastic: ?????? we should not allow the reparam here.
        * **how should we express that discrete states encode different future prob?**
    + emision stochastic: gaussian .
    

- KL loss. asks for no prior. 
    + transitional stochastic: there is a true prior.  How do we know it ? we don't need to know, we learn it?
    + emision stochastic: $\mathcal N(0, 1)$


## Dataset 
- v2
    + deterministic
- v3
    + 1, -1. 
- v4
    + continuous infinite number of states.
    + is guassian ok? is reparam ok?
    + **this seems fine for our model???**


## Problem of our model
- KL loss: instead of learning a distribution, it queeze all latent variable to 0...
- can the current LSTM capture two types of stochastic?? (in theory)
    + transitional: ok. but maybe we should not 
    + 
- if we want to capture these two kinds of stochastic, is long term variable a good choice?
