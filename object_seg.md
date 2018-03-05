# object segmentation
`Mar 5`

## intro
- Goal:
    + semantic seg
    + instance seg: just become more and more common
    + foreground, background
    + amodal seg: label all pixels, even the invisiable part: less common, _trend?_
- things(person) & stuff (grass, sky)
- _image parse Facebook_
- other application / connection
    + pose prediction -> seg
    + detection -> seg
    + 3D prediction -> seg. depth

## dataset 

|dataset | -- | -- | -- |
|---|---|---| ---|
| pascal voc | 20 | sparse | standard benchmark|
|COCO | 91 | sparse | new,much harder|
|NYU v2 | 40 | dense | has depth |
|ADE 20K | ?? | dense | parts labeled|

<!--     + pascal voc
        * 20 classes
        * sparse coverage
        * standard
    + MS COCO
        * 91 classes + instances
        * sparse coverage
        * new, nuch harder
    + NYU v2
        * 40 
        * dense
        * has depth
    +  ADE20K
        *  parts label -->

## evaluation
+ pixel accuracy
    * % correct
+ class accuracy
    * % correct, avaearged per classes
    * the fine details are hidden within small area.
+ IOU
+ sample around the boundary

## method
- two ingredients
    + indivisual pixel
    + consistency
- CRF
    + optimize over labeling of nodes y
        * $\sum \phi(y_i) + \sum \varphi(y_i, y_j)$ __maybe we can revisist it using graph?????__
        * pay penalty only if the adjacency pixel looks similar
        * NP-hard
        * with __right potentials__, feasible __????????__
    + How to construct graph
        * graph over super pixels - ocassinally appear
        * adjacencnt - almost disappear
        * every pixel - stil going strong (Fully connected CRF)

- convnet perform clf
    + FCN
    + blah blah blah...
    + __Learnable upsampling ??????__  stride 2, pad 1
    + the last layer of CNN output is not appropriate for seg output . The clf will throw away the fine details.
        * fuse all representation: 
        * s kiplayers 
        * Hyper columns
            - problem: should weight clfer be the same at every pixel location?
            - ideally different: have some bias. / too expensive
            - what if we encode location into hyper column? - only 2 channels, tend to ignore them.
            - compromise :  5 * 5 coarse grid clf


