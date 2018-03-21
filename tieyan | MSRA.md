## challenge
- big data 
- computational 
- automatic tuning model. learning to teach
- theory

## work
- leveraging structural duality in AI 
    + eg translation
    + dual learning - new learning framework
- Dual learning
    + dual unsup learning (NIPS  2016)
        * why work?
        * probabilistic nature P(x,y) = P(x)P(y|x;f)
    + dual inference (IJCAI 2017)
- Equivalence class0absed DNN optimization
    + problem
        * maybe SGD is wrong
        * redundancy in deep neural network(DNN) w1 * c, w1 / c
        * equivalent class in DNN space
    + magic
        * highly redundant weight space
        * map weight space to equivalent class space
        * SGD over path instead of weight
- light GBD (NIPS'16, 17)
    + gradient booosting decission tree(GBDT), when
        * feature are sparse 
        * goal is a decision making of forecasting
        * compare to XGBoost     