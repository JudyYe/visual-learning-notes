# scaling and benchmarking
`Priya` (webiste)[https://research.fb.com/people/goyal-priya/]


## Why self-supervised?

## Why scale up?
- very limited data: same scale of Imagenet
- How about 1M -> 100M??
- 3 axes
    + data
        * higher capacity model should be trained
    + problem complexity
        * colorization seems less sensitive to problem complexity
        * is predicting pixel right? will it saturate? `denpends on the task`
    + model
        * higher capacity model should be trained
- Jigsaw puzzle, colorization (classification), not fine-tuning
- Investigation setup task
    + linear SVM

## Pre-training domain & Transfer Domain
- It depends on (src / dst) domain / task.

## Benchmark self-supervised learning
- No consistent evaluation setup: due to appraoch? or task?
- principle: should Genearlize to many task given limited supervision
    + many task
        * object detection
        * surface normal 
        * visual navigation
        * low-shot image classification
        * classification, object & scene
    + full fine-tuning vs freeze the model and apply linear classifier on top
        * fine-tuning only evaluate how good the initilization.
        * BUT: what if a non-linear classfifier? no-parametric method? 


## Summary
- outperform on Surface normal 
- better / competitive on viusal navigation
- match performance on detection
    + why detection even w/o detection is better than clf?
    + FineTuning does not really help in DET
- worse on clf & low-shot clf








