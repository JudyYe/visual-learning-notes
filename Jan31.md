# Deep Learning(Intro)
## detection history
- HOG based, 0.1        , 2005
- DPM,       0.2->0.35  , 07-12
- R-CNN,    , 0.6       , 2014  --- learning feature

## what is deep learning?
- hand-design -> automatically learn feature
- ideal feature
    + non-linear
        * function family : too much.
        * we do not know what kind of function yet
- learn non-linear feature, (from dictionary of non-linear function $g_i$)
    + linear combination of  $\sum(g1, g2, ...)$
    + composition: $g_1(g_2(g_3...))$
    + comination and composition are the same power with infinite dictionary
    + but same volcabulary, composition is more complicated
- Hoever, optimization is hard. non-convex, non-linear.
- Claims
    + some are probabilistic
    + conv net is just one instance

##Deep NN 101

... blah blah ...
... blah blah ...

- vanishing gradients
    + why always vanish instead of exploding? 
        * activation
- activation
    +  sigmoid, 
        *  not 0-center - zig-zag
        *  saturated end
    +  Relu
        *  does not saturate
        *  converges faster! 6 *
        *  BUT not 0-centered
        *  some die -> sparse but some die


