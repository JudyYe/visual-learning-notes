# Adaptive adversarial learnign for a Diverse World
`[website](http://people.eecs.berkeley.edu/~pulkitag/)` `Feb 27th` `VASC`` Domain Adaptation`

## Motivation
- Benchmark Performance
- supervied only with label. but need to learn a huge param space.
- Whether we can assume, visual recognition will be solved ? or Image clf on Thounsands of classes has solved?
    + Assumption: same distribution 
    + Dataset Bias  
        * people bias when labeling. nice lighting, less obstacle
        * low reso, motion blur, pose variety

## How can we learn to generalize?
- domain adaptation: train on source test on target
- Not to retrain a new model
- classic domain adaptiaon
    + hand design function to extract feature of both 
    + distribution discrepancy
- learn a repersentation that cannot tell the domain
    + end to end
    + minimize discrepancy - 
        * max mean
        * higher order
        * dn discrepancy - probably upper bound the target error

## domain adversarial optimmization
- align domain in representation space
    + target does not have label
    + what prevent putting to zero? - we want to use the representation for clf
- align domain in image space
    + similar to conditonal GAN (but not the same)
    + eg. street house number -> MNIST GAN / cycle GAN -> no semantic constraints. (target semantic constraints are obtained from the source domain clfer)

## application
- digit recog
- Auto driving. 2017. adaptation of semantic segmentation
- fine-grained recogmnition
- task transfer, Luo, Zou, HOffman, Fei-Fei. NIPS'17
    + pariwise similarity
    + minimize the entropy of the similarity vector


