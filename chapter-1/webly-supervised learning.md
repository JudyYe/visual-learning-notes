# web-supervsied learning of visual representations
`Apr 18`

## intro
- setup(NEIL)
    + _image searching engines_
    + classes: iamgenet + NEIL
    + class name as queries and labels

## NEIL(life long learning system)
- more data or clean data?
    + google only < flickr + google < flickr
    + easy data is the key. hard one will crash the network
- higher-order constraints
    + one hot is not a good idea to represent the relationship between classes
        * XXX?? 很多 work see slides
    + staged + __graph__
        * ????
        * put regularization on class relationship
        * how to get graph: confusion matrix by simple model and easy data
- easy & hard definition?
    + curriculum learning
- conclusion:
    + __order__ matters: easy->hard 
    + __structure__ helps: graph
-

## lifelong
- if you learn one thing, it helps to learn the next things
- how to make it trustful
    + focus on high score (low recall but high precision)