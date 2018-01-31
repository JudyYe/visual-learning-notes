
# some theory
## David Marr - some turning point
* 4 stages of visual perception
    1. image-based, retinal based, edge, 2d, not exact
    2. surface-based, normal estimation, depends on viewpoint, 2.5d **?? is there fully possiible??? some info lost in edge detection**
    3. object-based, grouping parsing, viewpoint free, 3d
    `is it a bottom-up or top down?` 
    4. category-based representation
    `why people do category: it can relate the image to other meta info. because category follow some patterns in the world`
    `what kind of category is implict and can be different`

## curent pipeline (1990-2010)
1. Images - > 
2. low level -> 
    - SIFT, HOG, edge, blah 
3. midlevel (im)-> 
    - grouping
4. high level
    - sementation using the representation
- problem
    + the boundary between each stage blurrs
        * normally low-level -> directly goes to the high level stages
    + bottom-up? top-down?

## modern (2010 - )
- The boundary / info flow does not matter
- *end to end*, squeeze all middle stages
    + do not need to specify between 
info flows in feedforward (bottom up)
    `but not the same feedback as human > some problem`
    `top-down -> context drivens`


# how object recognition changes over the year
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



---

# the promise and perils of Big data
what is crucial about data?

## why do we need data?
- solve ambiguity - by frequency `rather than reason?????`

## how much data 
- what is more or less?
    + before: 
    + curent: 10^{6-7}, google / fb is about 100 times
    + reasoning --> matching problem
- human uses, visual long term memory: 
    + fidelity of images
    + 10k - so few??
    + what are people remeber??
    + have a surprisingly good / large memory, but also have a good transformation ability
































