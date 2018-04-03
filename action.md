### Mid-term
- introduce problem
- how you are going to solve
- no result expected

# understanding video
## goal
- given an input video, obtain an understanding
- put individaul element all together. 
    + object
    + human
    + action
- far far away
- SOA: detecting kick ball-30%

# Action Recognition  

## what is action/ activity
- is action just movement?
    + agent + __goal + intention__ + target state + etc
- SOA: most of SOA, are appearance based
    + no concept of motion
    + avearging result
    + no idea of what the problem is, what action is
    + how to represent time?
- term
    + gesture
        * single body part
    + action
    + interaction
    + group activity
- challenge
    + environment variation(separate background and other meaningful things)
    + actor movement variation - but actually detecting chair is also much variation: so it is not the main issue
    + biggest challenge: data
        * sports-1M
        * ucf-101
        * hollywood 2

## action work
- two - stream VGG
    + spatial + temporal
    + spatial - pretrain on imagenet 
    + temporal: optical flow, trajectory, 9k video is not enough
        * doom to overfit
        * combining dataset
        * very high dropout rate 0.9 
        * self -supervised
        * (fixing layer)
        * (data augument)
        Best Practice - dropout is better than reducing param number
- 2D- 3D convolution
    + 3d conv: move along depth as well.(instead of all in depth dimension)
    + main problem compared to 2-stream:
        * we cannot pretrain
        * we want to init 3D with 2D

- __State-of-art model__ i3D
    + introduce a large dataset:
        * KINETICS, 400 * 400 video, biggest one
        * init 3D by 2D
        * UCF-101 97.8

`sports 1M is not a good dataset to initizaize`
`LSTM cannot really restore long term memory, 2 hops, 3hops is farthest`

- action~transformation
    + action  = movement + goals
    + actions = transforming the enviroment according to agent's goals
    + features before * actions = feature after
    + training
        * precondition, effect, model transformation
        * ?? what are precondition??
    + inference
        * find precondition, effect
        * max(all transformation)
    + cross category generalization
        * long jump, high jump
    + approach
        * siamese

- non-local neural network



