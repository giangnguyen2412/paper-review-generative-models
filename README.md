# paper-review-generative-models
A hub for reviews of generative models

### 2020
* [Open Questions about Generative Adversarial Networks](https://distill.pub/2019/gan-open-problems/) - Augustus Odena - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/open_questions.md)

* [Image Processing Using Multi-Code GAN Prior](https://distill.pub/2019/gan-open-problems/) - Gu et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/mganprior.md)

### 2019
* [GANalyze: Toward Visual Definitions of Cognitive Image Properties](https://arxiv.org/abs/1906.10112) - Lore Goetschalckx et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/ganalyze.md)

### 2016
* [InfoGAN: Interpretable Representation Learning by Information Maximizing Generative Adversarial Nets](https://arxiv.org/abs/1606.03657) - Xi Chen et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/3.md)
* [Least Squares Generative Adversarial Networks](https://arxiv.org/abs/1611.04076) - Xudong Mao et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/4.md)

* [DC GANs - Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/abs/1511.06434) - Radford et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/5.md)


### 2015

* [Deep Neural Networks are Easily Fooled:
High Confidence Predictions for Unrecognizable Images](https://arxiv.org/abs/1412.1897) - Anh Nguyen et al, `CVPR` - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/1.md)

### 2014

* [Conditional Generative Adversarial Nets](https://arxiv.org/abs/1411.1784) - Mehdi Mirza and Simon Osindero - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/2.md)

* [Best explanation of GANs based on Information theory I've ever seen](https://medium.com/@jonathan_hui/gan-why-it-is-so-hard-to-train-generative-advisory-networks-819a86b3750b)


## Hack the GANs - Training tricks

- A stable GAN will have a discriminator loss around 0.5, typically between 0.5 and maybe as high as 0.7 or 0.8. The generator loss is typically higher and may hover around 1.0, 1.5, 2.0, or even higher.

- The accuracy of the discriminator on both real and generated (fake) images will not be 50%, but should typically hover around 70% to 80%.

- The -logD trick: When training the generator, we want to minimize log(1 - D(G(z))) (this has a form of log (1-x)). Using [graph calculator](https://www.desmos.com/calculator) we plot and see that the slope of this function is very small at first, thus giving handicaps for G when training in early stages. To solve this, we have to equalize the "minimize log(1 - D(G(z)))" to minimize -log(D(G(z))) (-log x). Using the graph plotter again, we can see the gradient at the early steps is much more stronger. By doing this, training GANs can be greatly improved.

