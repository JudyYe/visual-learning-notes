# learning single-view 3d reconstruction of objects and scenes

## skeleton
### How to perceive 3D from 2D??
using explicit priors
learning from annotation (implicit prior, occurance prob)
    - can we similiaryly learn 3D perception
        + NO!! Too costly and often wrong
learning via geometirc consistency
    provide collection of feedback
    --> multi-view reconstruction via geometric consistency        
        CVPR'17. Consider Geometric Consistency Loss!! L for different ground truth
        L (gt, output of 3D)
### What to perceive 3D from 2D?
structurely representation
compositionality