+++
showonlyimage = false
draft = false
# image = "img/papers/vae-schematic.jpg"
image = "img/papers/rock.gif"
date = "2022-09-01T19:59:22+05:30"
title = "R-VAE: Live latent space drum rhythm generation from minimal-size datasets"
weight = 15
categories = ['publication', 'featured']
tags = ['research', 'paper']
years = ['2022']
+++

Journal of Creative Music Systems

<!--more-->

[Gabriel Vigliensoni, Louis McCallum, Esteban Maestre, and Rebecca Fiebrink. 2022.  _Journal of Creative Music Systems 1(1)._](https://doi.org/10.5920/jcms.902)

### Abstract

In this article, we present R-VAE, a system designed for the modeling and exploration of latent spaces learned from rhythms encoded in MIDI clips. The system is based on a variational autoencoder neural network, uses a data structure that is capable of encoding rhythms in simple and compound meter, and can learn models from little training data. To facilitate the exploration of models, we implemented a visualizer that relies on the dynamic nature of the pulsing rhythmic patterns. To test our system in real-life musical practice, we collected small-scale datasets of contemporary music genre rhythms and trained models with them. We found that the non-linearities of the learned latent spaces coupled with tactile interfaces to interact with the models were very expressive and led to unexpected places in musical composition and live performance settings. A music album was recorded and it was premiered at a major music festival using the VAE latent space on stage.

MAIN FINDINGS AND CONTRIBUTIONS




{{< figure src="/img/papers/midi-24ppqn-cropped.jpg" alt="" >}}
<div class="text-caption">Data structure chosen to allocate simple and compound meter rhythms.</div>

The horizontal axis shows all 96 ticks in one 4/4 bar with 24 ppqn (pulses per quarter note) resolution. The y axis show standard subdivisions, where 4 indicates quarter notes, 8 indicates eight notes, 8T is used for eight triplets, and so on. The maximum resolution is a 32nd triplet note.

{{< figure src="/img/papers/vae-schematic.jpg" alt="" >}}
<div class="text-caption">Neural network architecture. The music input data goes into the encoder part of the network. When the latent space is sampled, datapoint are decoded into a symbolic music format.</div>

At training time, rhythmic data in symbolic music format is described in terms of their onsets, velocities, and microtimings, and encoded into a latent space. At generation time, a musician samples this space directly using a performance interface. The rhythmic patterns are then retrieved and decoded into a symbolic music format.




DINAMIC VISUALIZER
{{< figure src="/img/papers/diagram-visualizer.jpg" alt="" >}}
<div class="text-caption">Diagram illustrating the mapping from the latent space to the performance space canvas.</div>

 On the left, four discrete points (i.e., four rhythms) of the latent space are sampled over time, each represented in the figure as a 3-by-3 matrix. Each instrument in a rhythmic pattern will trigger a specific matrix cell with a single color. On the right, the full performance space, made of 900 points sampled from the latent space, is shown. Here, the visualization shows how the activation of different drum instruments (i.e., kick, snare, and hi-hat) differs across the latent space for this particular moment in time, t. A full measure consists of 96 of these images, played in sequence to produce a dynamic animation.
The user interface of R-VAE-JS web application is displayed on the right. The latent space can be explored by moving the mouse. Additional knobs for threshold and noise, as well as shortcuts to mute drum instruments allow the performer to interact with and control the web-based instrument. 

R-VAE IN MUSICAL PRACTICE
{{< figure src="/img/papers/devices-live-set.jpg" alt="" >}}
<div class="text-caption">Musical interfaces to control the latent space.</div>



The mapping of parameters to control R-VAE and the sound synthesis generation was implemented through three interfaces. The R-VAE decoding from the latent space was controlled through a Kaoss Pad XY grid, potentiometers, and buttons (the device in the middle). The interface of a Tempest synthesizer was used to control the drum sound parameters. Knobs and sliders in a third controller were mapped to the parameters of a physical model synthesizer.
<!-- {{< figure src="/img/papers/g1.gif" alt="" >}} -->

{{<youtube-custom id="Kib8Bk2nPEA" yt_start="200" autoplay="false" width="200px" height="200px" color="white" modestbranding="1">}}
<div class="text-caption">The video shows how the rhythmic latent space is  explored in real-time performance by means of interaction through MIDI controllers.</div>


