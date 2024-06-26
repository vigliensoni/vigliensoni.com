+++
showonlyimage = false
draft = false
image = "img/covers/ircam-2024-sq.jpg"
date = "2024-06-25T19:59:22+05:30"
title = "Weaving memory matter: Steering latent audio models through interactive machine learning"
weight = 10
categories = ['presentation', 'featured']
tags = ['talk', 'demo', 'performance']
years = ['2024']
+++

IRCAM, Centre George Pompidou, Paris


<!--more-->

{{< figure src="/img/covers/ircam-2024.png" alt="Taller Materia y Memoria" >}}
 

“Weaving memory matter” is a demonstration and performance where I will showcase the steerability and control of neural audio synthesis models through interactive machine learning. Real-time control in neural audio synthesis systems is important as it enables performers to introduce the long-term temporal coherence often missing in these systems.

Recent advances in neural audio synthesis, such as the RAVE architecture (Caillon and Esling 2021), have improved real-time audio signal generation. RAVE addresses issues of previous systems, including high computational complexity, poor signal quality, and short temporal coherency when modelling complex polyphonic audio signals. It also addresses the lack of interaction means. This progress has facilitated the use of these models in real-time performance. However, considering the potential large dimensionality of the learned embedding and the absence of labels for latent space axes, finding a better method for real-time interaction and performance remains crucial.

In this demonstration, I will present a useful method for steering neural audio models using interactive machine learning. This approach allows the performer to map the well-known, low-dimensional human performance space to the high-dimensional latent space of a generative audio model. This mapping is learned through a training set containing matched locations from both spaces.

During the demo, my process will include: (i) exploring the latent space of a pre-trained RAVE model to identify points of creative potential; (ii) selecting source points in the performance space that correspond to target points in the latent space; (iii) repeating these steps as required based on discovered sonic qualities; and (iv) using a regression algorithm to learn a mapping between points in both spaces. This process can be repeated as needed for adjusting the mapping.

In the demo performance “Weaving Memory Matter,” my goal is to demonstrate how we can reclaim artistic control over generative AI systems by training custom models on curated data and steering the generative process. The performance utilizes a RAVE model trained on part of the sound archive of Santiago de Chile's Museo de la Memoria y los Derechos Humanos. Technologies used include RAVE, nn~, Facemesh, FluCoMa, and Max.


[IRCAM link](https://forum.ircam.fr/article/detail/weaving-memory-matter-steering-latent-audio-models-through-interactive-machine-learning/)




{{<youtube _czEdig5BNo>}} 

