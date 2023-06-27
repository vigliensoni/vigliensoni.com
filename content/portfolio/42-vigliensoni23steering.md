+++
showonlyimage = false
draft = false
image = "img/papers/ICCC2023-V3-dean.gif"
date = "2023-06-20T19:59:22+05:30"
title = "Steering latent audio models through interactive machine learning"
weight = 11
categories = ['publication', 'featured']
tags = ['research', 'paper']
years = ['2023']
+++

14th International Conference on Computational Creativity

<!--more-->

[Gabriel Vigliensoni and Rebecca Fiebrink. 2023. In _Proceedings of the 14th International Conference on Computational Creativity (ICCC 2023)_.](https://doi.org/10.5281/zenodo.8087978)

ABSTRACT

In this paper, we present a proof-of-concept mechanism for steering latent audio models through interactive machine learning. Our approach involves mapping the human-performance space to the high-dimensional, computer-generated latent space of a neural audio model by utilizing a regressive model learned from a set of demonstrative actions. By implementing this method in ideation, exploration, and sound and music performance we have observed its efficiency, flexibility, and immediacy of control over generative audio processes.

The video below shows our approach instantiated through a RAVE model trained on a large dataset of acoustic harmonic audio signals. The model has eight latent dimensions. A 2-dimensional human performance space is mapped to the RAVE (Caillon and Esling 2021) model through regressive model using FluCoMa (Tremblay et al. 2021)


{{<website src="https://media.vigliensoni.com/video/iccc2023">}}
<div class="text-caption">Supporting video demoing the proposed approach to steer latent audio models. </div>

### References

Caillon, A., and Esling, P. 2021. RAVE: A variational autoencoder for fast and high-quality neural audio synthesis. arXiv:2111.05011.

Tremblay, P. A.; Roma, G.; and Green, O. 2021. Enabling programmatic data mining as musicking: The Fluid Corpus Manipulation toolkit. Computer Music Journal 45(2):9–23.