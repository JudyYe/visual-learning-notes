# On Challenges in Image Geneartion
`[website](http://lihi.eew.technion.ac.il/)` `Feb 20th` `VASC`

## application
- stytle transfer
- single image animation
- gender change

## Problem 1: current loss
- pixel loss 
    + require alignment
- Gram loss(global statistics)
    + fail when style transfer
- __problem 1 : some loss__
    + not require alignment
    + region compare of semantic part

## Template matching
- related 
    + template matching
    + best-buddies similarity(BBS) Dekel, Oron 2015
        * NN within patch + bi direction
        * robust in deformation, occlusion
        * deformation field???
- approches
    + template matching matching with deformable diversity similarity, cvpr'17
        * only one way
        * find deformation field
            - positive: short 
            - negative: long

## Use the loss in image generation
- deva: `how to make it differentiable?`
    + soft version of Counting_????????_
- results
    + used in applications
- application
    + gender 
        * cycle gan
        * A1: `generailization of their method? face is narrow space`
- How to make more real?
    + distribution of gradient

