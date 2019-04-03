# context

## intro
- context modify human's perception
- double edges sword
    + the less resolution is, the more helpfule context is


## why context is important
- resolve ambiguity
- notice unusual things

## kinds of context
they try to model in the past

- semantic context
    + see a scenee: very likely to coocurrance together
- geometric context: 近大远小
- temporal context
    + smooth over time
    + recognition 
- cutural context??
    + male / female standss

## context models - all Prob Graph Model..
- correlated via scene 
- dependencies among objects
    + low level output statistics - contextual priming. 
    + model geometry of the scene CVPR 2017


## works
- contextual priming for object detection
- modling the viewpoint and surface geometry
    + 1st rule: scene geometry <--> object support (object must be supported)
    + 2nd viewpoint rule: horizon line <--> __object size__
    + dramatically reduce the search space

## context in deep learning
`Shrivastava, Abhinav, and Abhinav Gupta. "Contextual Priming and Feedback for Faster R-CNN." ECCV, 2016.`

- where can i get the feedback? (what layer that you know it is office desk?)
    + segmentation
        * compact, easy to represent
        * capture contextual relationships between ojects
- where should i put my feed back?


## context as knowledge graph
`Marino, Kenneth, Ruslan Salakhutdinov, and Abhinav Gupta. "The more you know: Using knowledge graphs for image classification." arXiv preprint arXiv:1612.04844 (2016).`

`Li, Ruiyu, et al. "Situation recognition with graph neural networks." arXiv preprint arXiv:1708.04320 (2017).`

- relationship graph.  
    + eg. easy to detect skateborad -> deduce the person is wearing jeans instead of pants
    + pass message among node (belief propagation)
- latent variable representing node
- initialize the latent variable?
    + faster-rcnn
    + fc7 feature vector
- slowly expand the nodes, instead of see the graph in one shot.




