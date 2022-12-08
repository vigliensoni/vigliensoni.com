+++
showonlyimage = false
draft = false
image = "img/papers/R-VAE-1.jpg"
date = "2022-05-04T19:59:22+05:30"
title = "Creating Latent Spaces for Modern Music Genre Rhythms Using Minimal Training Data"
weight = 19
categories = ['publication', 'featured']
tags = ['research', 'paper']
years = ['2020']
+++


<!--more-->

[Gabriel Vigliensoni, Louis McCallum, and Rebecca Fiebrink. 2020. In _Proceedings of the 11th International Conference on Computational Creativity (ICCC’20)._](https://doi.org/10.5281/zenodo.7415792)

In this paper, we present research on customizing a variational autoencoder (VAE) neural network to play with musical rhythms encoded within a latent space. To enable customization and personalization, the network can be trained with as few as one dozen MIDI clips with rhythms.
Additionally, our approach employs a data structure that is capable of encoding rhythms with binary, ternary, or a combined metrical grid. A metrical grid can be explained as the main ratio by which the onsets of notes are placed in a measure. Music where the beats are split in two—a binary grid—is in simple meter. Music where the beats are split in three—a ternary grid—is in compound meter. Many modern music genres, such as footwork, gqom, dembow, or trap, can be characterized by rhythmic elements using a compound meter. In these rhythms, the main meter is usually simple but there are elements that are placed on an overlaid ternary grid. To the best of our knowledge, this work is the first time that a network architecture has been used to encode rhythms that exhibit a combined binary and ternary grid.


{{<website "https://underline.io/lecture/2780-creating-latent-spaces-for-modern-music-genre-rhythms-using-minimal-training-data">}}
