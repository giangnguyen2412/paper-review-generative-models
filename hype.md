# HYPE: A Benchmark for Human eYe Perceptual Evaluation of Generative Models

## Summary

Generative models often use human evaluations to measure the perceived quality
of their outputs. Automated metrics are noisy indirect proxies, because they rely
on heuristics or pretrained embeddings. However, up until now, direct human evaluation strategies have been ad-hoc, neither standardized nor validated. Our work
establishes a gold standard human benchmark for generative realism. We construct
HUMAN EYE PERCEPTUAL EVALUATION (HYPE), a human benchmark that is
(1) grounded in psychophysics research in perception, (2) reliable across different
sets of randomly sampled outputs from a model, (3) able to produce separable
model performances, and (4) efficient in cost and time. We introduce two variants:
one that measures visual perception under adaptive time constraints to determine
the threshold at which a model’s outputs appear real (e.g. 250ms), and the other a
less expensive variant that measures human error rate on fake and real images sans
time constraints. We test HYPE across six state-of-the-art generative adversarial
networks and two sampling techniques on conditional and unconditional image
generation using four datasets: CelebA, FFHQ, CIFAR-10, and ImageNet. We find
that HYPE can track the relative improvements between models, and we confirm
via bootstrap sampling that these measurements are consistent and replicable

 The first, called HYPEtime, is inspired directly by the psychophysics
literature [28, 11], and displays images using adaptive time constraints to determine the time-limited
perceptual threshold a person needs to distinguish real from fake. The HYPEtime score is understood
as the minimum time, in milliseconds, that a person needs to see the model’s output before they can
distinguish it as real or fake. For example, a score of 500ms on HYPEtime indicates that humans
can distinguish model outputs from real images at 500ms exposure times or longer, but not under
500ms. The second method, called HYPE1, is derived from the first to make it simpler, faster, and
cheaper while maintaining reliability. It is interpretable as the rate at which people mistake fake
images and real images, given unlimited time to make their decisions. A score of 50% on HYPE1
means that people differentiate generated results from real data at chance rate, while a score above
50% represents hyper-realism in which generated images appear more real than real images.
