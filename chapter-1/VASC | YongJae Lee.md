#  Learning to localize and anonymize objects with indirect supervision
`VASC`, `Yong Jae Lee`, `Oct 8`, `[website]`(http://web.cs.ucdavis.edu/~yjlee/)

## Motivation 
- Bottol neck of Scale up?
    + he claims to be __DATA__ of direct supervision: 
        * labor heavy
        * what to annotate? 
        * How to label? annonymization for privacy.


## localize
Hide-and-Seek: Forcing a Network to be Meticulous for Weakly-supervised Object and Action Localization
- problem: only focus on the most discriminative part
- method:
    + masking pixels randomly
- why not Adversarial???
    + random is efficient
- visualization tool
    + Bolei CVPR'16
- what shall the value of hidding pixel be?
- QA: 
    + metric: mAP at pixel level
    + how important is the hyperparam? 
- Application:
    + use it as Data augmentation.



## [Anonymize](https://jason718.github.io/project/privacy/main.html)
- motivation
    + privacy
- method
    + adversial
    + detecting face -> 
        action detector + face classifier
- QA
    + why consistency?





