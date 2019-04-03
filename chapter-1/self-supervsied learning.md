#self superised learning
`Apr 4`

perspective of ML

## argument
- not human-like
- engineer: supervised unscalable
- what if we don't need to scale up for supervised?
    + nobody shows more than 1 Million images help
    + what if the curve saturate?

`scale learning by building self-supervsied system`

## how to get supervision without label?
### motivation: supervsied learning 
- pls learn a network that will hopefully can learn to factorize some informatino
- though the network are trained by the task of clf, but it generalizes well to other tasks!
- most tasks are related to each other.

## pretext tasks
- related to semantics but gt is free.

### self-supervised vs unsupervsied learning
- different from unsup
- learn a generative model: p(x, y) sample new example
    + can generate new data, GAN
- self-supervsied: still try to learn discriminative model p(y|x)
    + competitive result on vision tasks, det, seg, etc

### scale range (many paper... 15 papers)
- images
- videos
- sound depth
- actions


## evaluation
`Pathak, 2017` comprehensive evaluation

- how good the representation?
- what is a good representaiton?
    + NN
    + activations of neurons
    + quantitatively, fine-tune on top and do standard task
        * will ft take the credit?
        * ft last few layer and still work
            - you can hardly say what happens in ft.....
        * use less data and still work

## some works
- from image
    + re-color
        * ambiguity, multiple output
        * network tends to average out the multiple output, with L2 loss
            - multinomial clf. but not all color are equally likely
    + context, carl
        * monivation: word2vec: skip-gram
        * avoid trivial shortcut: jittering
        * they can even directy predict the absolute position: chromatic aberration....... 红波焦距长。。。。
        * random initalizetion NN still make some sense: some prior in architecture.
    + jigsaw
    + inpainting
    
- from video
- invariance aspect
    + multitask
    + transitivity in invariance.
-  from audio
    +  predicting sound
        *  altough lowest performance
        *  a complementary to image-based method
-  from 3D
    +  depth
-  from action
    +  ego motion
    +  robotics
        *  instance level image retrieved task: __beat Imagenet!!__

# one problem of self-supervised approaches
- how to evaluate
    + some learn sth useful, but not as good as ImageNet
    + we are playing the games of imagenet
    + but the representation learning is broader than semantic task(e.g. detection, segmentation)
    + scene recognition / normal estimation

## big phylosiphy discussion: does more data even means better representation?
- questions
    + what happens at 100x?
    + plateauing effect?
    + data vs model capacity
- answer1: empirical study
    + JFT-300M dataset - google
        * unknow recall
        * heavily long-tailed
        * 20% noise
    + Imagenet -> JFT-300M
        * 4 epcoh 1.5months, 
        * not so much improvement, on 
    + datasize vs performance: log-linear
        * large scale data plays crucial role here.
    + deep vs performance
    + We need both model and data

