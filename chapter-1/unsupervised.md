# unsupervised learning

## intro
- self-sup vs un-sup
    + x = [x1, x2] : x1-> Model ->x2'
    + self-sup is still discriminative learning, generative P(X)
-  motivation
    +  we learn via loss-function -> can we learn without any labeled data?
        *  labeled data is human upper bounded
        *  unscalable

## method
- stacked autoencoder
    + too much shortcut the model can learn
- denoising AE
- AE basically learn a manifold, but suffer from multiple correspondence / reconstruction, not aligned with semantic meaning
    + -->> VAE