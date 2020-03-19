# paper-review-generative-models
A hub for reviews of generative models

### 2016
* [InfoGAN: Interpretable Representation Learning by Information Maximizing Generative Adversarial Nets](https://arxiv.org/abs/1606.03657) - Xi Chen et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/3.md)
* [Least Squares Generative Adversarial Networks](https://arxiv.org/abs/1611.04076) - Xudong Mao et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/4.md)

* [DC GANs - Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/abs/1511.06434) - Radford et al - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/5.md)


### 2015

* [Deep Neural Networks are Easily Fooled:
High Confidence Predictions for Unrecognizable Images](https://arxiv.org/abs/1412.1897) - Anh Nguyen et al, `CVPR` - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/1.md)

### 2014

* [Conditional Generative Adversarial Nets](https://arxiv.org/abs/1411.1784) - Mehdi Mirza and Simon Osindero - [review](https://github.com/luulinh90s/paper-review-generative-models/blob/master/2.md)

## Problems in training GAN
### Hard to achieve Nash equilibrium
### Low dimensional supports
### Vanishing gradient
### Mode collapse
### Lack of evaluation metrics

## Hack the GANs - Training tricks

- A stable GAN will have a discriminator loss around 0.5, typically between 0.5 and maybe as high as 0.7 or 0.8. The generator loss is typically higher and may hover around 1.0, 1.5, 2.0, or even higher.

- The accuracy of the discriminator on both real and generated (fake) images will not be 50%, but should typically hover around 70% to 80%.

