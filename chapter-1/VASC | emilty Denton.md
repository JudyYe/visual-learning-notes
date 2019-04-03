# Towards Better Methods of Video Prediction

## chanllenge
- what is representation space ? abstract space
- what does it used for? precise? high level?
- uncertainty in the world

## Content and Pose 
- content: anything predictable from past frame
- the goal here is mostly interpretable latent feature.
- pose: 
    + scene discriminator: cannot distinguish which video clip it comes from - pose unalignment. distribution should match. 
    + stack falling? number of the object changes?
    + local linealiy: change linearly across small step
- applicaition
    + image dsynthessi by analogy: A content + B pose 
    + interpolation
    + VIDEO PREDICTION: LSTM in pose space.
        * do not feed back error from pixel space to back prop
- fixed number of object: moving MNIST, KTH video......
- pose across video???
- explictly requires the clean separation of conetent and pose

## Stochastic Video Generation with a Learned Prior
- chanllenge:  averaging possible future...
- latent z: capture anything that cannot be captureed from the past
- key : for soeme segments of the video deterministic model may suffice. some part is more deterministic.
    + learn prior in encoder
    + let decoder deal with the prior
- prior: $\mu, \sigma$.

- location

BAIR robot push sequence: 30

## QA
- dataset
    + super simple / way too hard
    + similar model: 
    + a set of datset : one reflect an aspect
    + long term motion, interact, lighting condition.
    + more annoataion.
- factorize in terms of spatial 
