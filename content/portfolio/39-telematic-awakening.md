+++
showonlyimage = false
draft = false
image = "/img/papers/audiostellar-inv-2.gif"
date = "2021-11-19T19:59:22+05:30"
title = "Telematic awakening"
weight = 30
categories = ['music', 'research', 'featured']
tags = ['research', 'single', 'release']
years = ['2021']
+++

<!--more-->

Telematic awakening: Participating in the 2019 Chilean uprising through a live gestural interface. 26th International Symposium on Electronic Art. Montréal, QC. 

ABSTRACT

The _Telematic awakening_ project was a way of participating in the 2019 Chilean uprising from abroad. I collected interviews and field recordings of the manifestations posted from social media feeds. The recordings were split into sound snippets, sound features are computed, and dimensionality reduction was performed so that the sounds were mapped into a bidimensional performative space. I used a motion tracker device and a machine learning system to capture and map hand positions into the sound space. Sound snippets in this space were concatenated in real time. The interface allowed me to participate telematically in the manifestations by creating layers of other people’s sounds on top of rhythmic and intense music as if I were fighting in the streets.

MOTIVATION

Tens of thousands have been taking to the streets in Chile since last October. People protest against inequality, increased cost of living, privatization of health and education, miserable pensions, and state repression. The unrest was triggered by student-led protests against a metro fare hike. Violence erupted after police fired teargas and water cannon at demonstrators. Some protesters responded by throwing petrol bombs. 

{{<figure src="/img/papers/telematic-manifestation-1.jpg" alt="Large manifestation">}}
<div class="text-caption">Tens of thousands in the streets in Chile in October and November 2019. </div>


State of emergency and curfew were declared. Army and tanks were sent to the streets in most of the country. In response, the protests broadened into a nationwide uprising and turned increasingly violent. The Chilean government announced a series of social reforms to appease the unrest but protesters say the reforms fall short. Dozens of people have died and more than 10,000 people have been arrested since the unrest began. 


{{<figure src="/img/papers/telematic-manifestation-2.jpg" alt="Police brutality">}}
<div class="text-caption">Heavy police repression.</div>


I have been witnessing the uprising from abroad the country but have been pretty much hooked to what is going on and wanting to participate and fight for our rights.


SOUND CORPUS

Thanks to ubiquitous mobile phones, there is a very large number of first-person recordings taken directly from the streets where the manifestations are happening. Protesters post these recordings on social media from where we can watch and listen them before these are taken down.

Very diverse type of sounds can be heard during the demonstrations: 

**Field Recordings**. A number of sounds can be heard in the demonstrations. Most people protest from their own homes making noise by banging pots and pans in order to call for attention in a pacific manner. Protesters sing chants and shout slogans when attending manifestations in the streets. Police react by firing water cannons, teargas, and rubber bullets. The most violent protesters also make barricades to stop police. Some of these barricades have created massive fires. Sirens from police trucks and fire engines are com-monplace in the manifestations.

**Historical Recordings**. I have also collected some of the interviews of Salvador Allende, the first socialist president in the world that arrived to power by democratic means in 1970. Most of his memories have been erased after the coup d'État led by Pinochet in 1973 and his dictatorship until 1990. The lucidity of the interviews and message seem completely pertinent to the current state of affairs, almost 50 years after they were made.




LIVE INTERFACE

For _Telematic awakening_, I play with the two sound corpora in a different fashion. While the field recordings are split into sound snippets of a specific short length, so that when looped they are synchronized to the tempo of the piece; the historical recordings are split by phrase, so that the message they convey is always understood. Hand positions and gestures are acquired and mapped to the sound corpora. At performance time, I adjust the position of hands using acoustic feedback to play sounds of the same, or different, type.

To play sounds, I decided to use AudioStellar (Garber, Ciccola, and Amusategui 2020). Field recording sounds are loaded into AudioStellar and characterized by specific audio features. This high-dimensional representation is then collapsed by the software into two dimensions. The resulting low-dimensional representation is convenient for sound distribution in space and sonic exploration. 

{{<video autoplay="false" loop="true" controls="true" src="/videos/audiostellar.mp4">}}
<div class="text-caption">Sound corpus loaded into AudioStellar</div>


After I assembled my sound corpus, I had to develop a way to interact with it. 

Hand positions and gestures are acquired by the Leap Motion hand tracking device and Open Sound Control messages outputted by this device are parsed and rerouted us-ing Max/MSP. The Wekinator, an application for real-time supervised machine learning interaction, is used to learn gestures and positions and map them to specific zones in AudioStellar sound space.

{{<figure src="/img/papers/telematic-diagram.jpg" alt="Schematic of mapping hand gestures into sound corpus">}}
<div class="text-caption">The figure shows the basic mechanism of interaction.</div>

On your right, you can see that audios in the sound corpora consist of field recordings and historical recordings. These audios are split into short snippets, which are projected into a latent space of sounds. Then, on your left, you can see that the position of the hands of the performer are acquired in the performance space, and mapped to the sound snippets.

PERFORMANCE


{{<youtube YXoA0hHQzEY>}}
<div class="text-caption">The video shows the sound corpus and the tools in action in the making of Telematic Awakening.</div>

I premiered the track live at the 2020 MUTEK Festival in Montréal.