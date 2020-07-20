# Image Processing Using Multi-Code GAN Prior

## Summary
Previous methods typically invert a target image back to the latent
space either by back-propagation or by learning an additional encoder. However, the reconstructions from both of
the methods are far from ideal.

In this work, we propose
a novel approach, called mGANprior, to incorporate the
well-trained GANs as effective prior to a variety of image
processing tasks.

In particular, we employ multiple latent
codes to generate multiple feature maps at some intermediate layer of the generator, then compose them with adaptive
channel importance to recover the input image.

The resulting high-fidelity image
reconstruction enables the trained GAN models as prior to
many real-world applications, such as image colorization,
super-resolution, image inpainting, and semantic manipulation. We further analyze the properties of the layer-wise
representation learned by GAN models and shed light on
what knowledge each layer is capable of representing.
