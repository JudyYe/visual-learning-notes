# Deep Learning(Intro)
`Jan31` `Feb5` `Feb7`
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


##Some notes
- Memory
    + weights
    + input
    + activation map
- Initialization
    + Xavier
        * var(X), var(Y) remain similar
- Normalization
    + Batch Norm
        * what is D??? Every dimention??? 
- Training check
    + regularization is not too strong
    + loss and gradients are correct
    + __should overfit on small dataset__ make sure you can overfit to the strong amount of data - very low loss.
- Training debug
    + loss does not go down: lr too low
    + loss explodes: lr too large
    + look loss curve
        * `Slides`
        * linearly goes donw: low
- Other tricks
    + momentum
    + Adam - very recent, people use it
    + `decide lr by hand improves more significant for Adam, blah, blah`
    + regularization
        * dropout: 
            - some redundancy in representation. if some path dies, there are others
            - maybe just ensemble
            - 0.5 is normal; but in action classification, people will use 0.9 (because optical flow are easy to overfit); Resnet: no dropout
        * weight decay
        * data augmentation
