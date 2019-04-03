# how object recognition changes over the year
`Jan24`
## geometirc era - recognition by component
- ecological theory -> understanding everything in the world
- some reasons
    + invariance to viewpoint
    + invariance to illumination
        * because is based on edges and contours, robust to illumination
    + man-made world
        * especially when all the object are man-made, from CAD
    + math can serve as solid tool
- classic work
    + block recognition 
        * reasoning, line label
        * `why?` not so many data
    + generalized cylinders. curve primitives
        * sweep of circle
    + geons, generalized geometric primitives

- hard prolem for them - so many assumption **but not impossible to solve**
    + modeling problem
    + clutter background
    + occlusion

## aspect graph
- key idea
    + generalized edge
    + modeling views rather than full geometry model
    + build graph to connect different views
- some reasons
    + supported by some psychologist
- hard problem
    + expensive to build graph, unscalable

## alignment 
- key idea
    + find transformation that fits the model
- some reasons
    + easily solve occlusion
    + top-down - u have a model, and match them
    + can enforce some invariance
- problem
    + generalized, in real world cannot work

## global appearance (data-driven)
- clasic work
    + eigenfaces
        * data starts to say what matters to this task
- problem
    + requies alignment 
    + clutter, occlusion

## local apperance
- classic work
    + bag-of-word
- problem
    + spatial structure
    + background foreground

## sliding window
- classic work
    + spatial pyramid
    + deformable part model
    + HOG

## parts and shape `!!!!!!!!!!!!!`
object as a set of parts
relative locations between parts (`spatial graph????`)

## RETURNS of CNN
- developed in 80's
- `video understanding still reamain a challenge`    state-of-art: 20% - 25%
    + temporary - time axis is different from spatial 
    + cannot be handled by convolution now. 
    + time is one way. 
    + causality
    + the current best way -> average
    + 3D conv -> some argue that the crucial part is not 3D conv.

## what's next???
return of geometric???
- physics and higher-level understanding
    + return to modeling blocks
    + synthetic 


