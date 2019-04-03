# the promise and perils of Big data
`Jan29`
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
- experiment
    + human can surprisingly remember category, exemplar, even state. 
    + human can remember all the details
    + --> computer should use as much data as we use
- scaling
    + lena
    + face, car
    + 1st standard benchmark dataset: PASCAL VOC. **2007**. 
    + vision move forward because of the benchmark
    + 10^5 
        * PACAL
        * Catech 101 and 256, image-level label
        * Lotus Hill Research Institute image corpus - deformable part (Songchun Zhu)
        * LabelMe, MIT, 2005 online. 530k object annotations collected
            - no consistency, no quality control
            - long-tail: follow the distribution of object in our real* world
    + 10^6-7
        * dowloading image using search engine
        * imagenet
            - CLEAN, cleaning up by crowd sourcing
            - `?how to control quality?` - money ...
            - now we know that we do not need so much clean data
    + 10^8-11
        * internet images, but noisy. 
        * human see in 10 years


## when do we need big data?

### dynamic equation?
eg, how the smoke spread
In this case, we do not need much data

### attributes!
- cannot really list
- eg, human psychology, genetics, economics. 
- cannot model `for now??` with math
- sometimes. simple alg + lot data > complex alg
    + does not mean that complex alg is less preferred. it's sometimes simple + much data will almost get u there
    + eg. machine translation
        * basically find the words used to appear in whole French 
        * state-of-the-art, until 2013/2014
    + eg. texture synthesis
        * nearest neighbor, copy paste


## How to use
- brute force vision
    + `nearest neighbor` and copy paste.. easy side
        ``non-local filter, context``
        * eg. colorization, 
        * eg. im2gpus (20M imgs)
        * eg. image completion (James Hays, AA Efros, 2007)
        * eg. nips'07
    + **KEY**: similarity metric
    + How to make *similarity* robust even with some 'not boring' scene
        * eg. paris in snow
        * learn? 
        * `attention mask` / reweight
            - eg. 吴哥窟
            - rareness - exemplar svm - weightness -> reareness / importance
    + How to make *alignment / warping* robust
        * HOG like scene parsing
        * eg. transfer segmentation annotation - (just retrieve best match by some metric, and then wraping their annotations)
    + use primitives
        * analogous: translation
        * eg. normal estimation
    + understand simple first
        * eg. pose detection of pitching video. Deva, Zisserman, 2004
        * eg. scene sketch understanding
- **Key idea**: "Maybe when u think your deep learnign works, it just can memorize large enought dataset "

- learn some pattern(This course focus)
    + move from CNN
        * learn manifold, parameter function


## Some Important  data observations

## distribution
- category
    + uniform vs long-tail :  LabelMe vs Imagnet
    + `Open Problem`: long-tail data, not forget about the tail

- Bias
    + From Search engine: eg. cup handle / viewpoint
    + eg. 'Name that dataset'
    + eg. Mixing datasets






































