# Recovering a Functional and 3D Understanding of Images
`[website](https://people.eecs.berkeley.edu/~dfouhey/)` `Mar 8h` `VASC`` Function` `3D`

## motivation
- boost: Naming things
- but naming is not enough
- need to recover 3D info
    + not only need learning but also need to undertand __3D__ representation
    + not only class, also __interaction__

## 3D representation
- goal: image- > 3D
- 3D representation
    + depth
    + surface normal
    + voxels
- RGB__D__ as supervision
- unsup learning, just using regularities.
    + supervision: _Vanishing points_~~
    + factorization: 2 component
        * structure & style
    + hwo to divide:
        * vanishing points + element detection
        * orientation + detection  / location
    + how to solve ambigurity
        * prior: average over the dataset
    + how to find element
- rgbd -> voxels
    + 20 * 20 * 20
    + train on syntetic, but transferable to real images
- scene (advanced) voxel
    + problem with one whole big voxel
        * cannot separate object
        * confaltes shape and pose
    + method:
        * factored, layout + per-object
        * bbox + per-object voxel - like mask-rcnn
        * using context & formulate rotation as clf rather than regression

## Interaction
- people as active sensor
    + eg. see a people siitnig at a dark sofa, changes your prediction of the scene
- problem: 
    + algorithm limited
    + data, sources limited
- using functional maps, 
    +   appearnce alone,  vs people 

### how to collect data?
- standard: explicit searching
    + failure: 'open up a laptop'
- their method: __implicit__
    + `VLOG`
    + Crowd sourcing

## Future
- functinoal models
- task-driven 3D
    + 3D representation -> robotics / high-level vision (differnt fields)
- video learning    
    + one variable changes - so few things change.  单一变量


## Q&A
- physically interacint vs sit and watch
    + pixel itself does not tell story. But it does if you know a little bit of eg. 3D
- common sense statictically?
    + learn structure
- how to representation function?
