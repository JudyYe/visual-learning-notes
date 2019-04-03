# see and think

## goal
- tackle perception(see) and reasoning (think) at the same time
- incooperate pttern recognition, symbols and search

## 2011->2018
- informative label
- 2012 Alexnet, CNN, end-to-end (whole learnable)
- visual KNOWLEDGE BASE (dataset)

## how to build imagenet
- small / lacking human label
- cleaning up by A(mazaon)MT(urk) worker
- quality control algorithm
- robust, scalable, clean

## resaoning (HEX)
- motivation
    + softmax
        * score-> probability
        * 互斥的
    + hierarchy and exclusion graph of label relation
- wordnet ontology
- replace softmax with another layer
    + probability constraints P(dog) > P(柯基)
    + define a probabilitic model
        * use raw score to define a joint probability districtuion(exp expode???)
        * use graph to zero out
        * ??
    + generic CRF. 
        * exclusions are good, we do not need to enumerate?? , clique
        * sparse graph are good: dynamic programming
        * equivalent graph, logical deduction

##  scene graph(hourglass) (associated embedding)
- `recognizing object is not enough` `but interaction`
- edge: interaction
- chalenge
    + deal with multiple object
        * keep fine detail(because feature map is low resolution)
        * ???vectorize a image
    + ???
- result
    + visual genome
    + recognizing iteraction
- idea
    + pixel to graph!!!
- by product
    + object detection reformulated

## future work
- pixels to 3D
    + crowd sourcing
    + RGBD is limited to certain scenes
- pixels to theroy of mind(people, animals, robots)
    + plan, goal, intention, belief
- commen sense knowledge space
    + what hsould be included in commen sense?
    + how to represent common sense?
    + where to acquire common sense?

- learning graph-based formula embedding NIPS'17
- textual QA

