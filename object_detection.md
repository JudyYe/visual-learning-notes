# Object Detection
`Feb19`

## How hard?
- deformable
- illumination

## History
- edge templates + NN
    + canny detector and matching
        * little learning
        * fail when too much edge
- hand designed features + ML   
    + form detection as classification problem
    + sliding window approaches
    + 1st method that somehow works: AdaBoost + rectangualr differential features(Harris feature).
        * they are fast
        * cascading classification to save computation
    + HOG
    + SVM
        * unbalanced data
        * __hard negative mining__
            - svm1: random sample
            - hard negative: svm1's False Positive -> svm2 -> ... -> svmn
            - _prevent forgetting_: preserve support vector
        * vs cascading method: it aims to save computation, not unbalanced data
- Using part-based model
    + some part can be non-semantic
        parts are learned
    + learn:
        * what are the part?
            - 5 part + root part(whole object)
        * what appearance of each part
        * location of the part
            - learn the relationship respect to the root part
        * __Score__: independent response + __deformation function__ `hmmmm. relative location`
        * How to define a part?
            - EM- style learning
            - given bbox on location and parts learning <--> given DPM models, localize

## Evaluation
- iou
- AP
    + AP^{0.5}, AP^{0.75}, AP^{0.25} - AP when iou > n

