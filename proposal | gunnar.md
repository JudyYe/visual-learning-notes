# human

## challenge 1: data
- the internet conatains exciting not daily video
- process
    + mining video internet 
    + labling with language
    + acting
- findings
    + confusion when the activeity happens
    + confusion with activity than object
- cattegory, object, action, prgress, scene

## challenge 2: algorthim - how to hardness the data
- evolution of activity
    + space time intersted points
    + trajectroies
    + dense trajectories
    + two-stream
    + c3d
    + lstm
- now
    + activeityies, not just motion
    + story summary
        * model the temporal structure of human activeities
        * skip the sequence and find important step -> reason of the sequence
    + what is activiety?
        * intent
        * object
        * human
    + Graphical model to model the structure
        * potential of graphical model
        * deep CRF 
        * temporal reasonaing: updating belief over time
        * converge smoother...
        * learning intent
            - one vector to encode intent
            - clutstering -> see some semantic meaning
- analysis
    + comprehensive
    + large categories have additional complexity
    + NO balanced data!
    + throw away 

## challenge 3: moving forward
- theory of mind
    + put ourself into other's shoes
- 1st 3rd person view
    + paiers of 1st / 3rd person videos via crowdsourcing
    + two times: not identical
- challenge
    + hard moment: person disappear, blurry
- learn what to learn from
    + distance between (3rd, 1st correct coorresponding frame) < (3rd, 1st wrong)
    + selector and training loss??
    + lean a shared representation to link the two views


## challange

