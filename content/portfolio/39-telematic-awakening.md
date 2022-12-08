+++
showonlyimage = false
draft = false
image = "/img/papers/telematic-diagram.jpg"
date = "2021-11-19T19:59:22+05:30"
title = "Telematic awakening"
weight = 30
categories = ['music', 'research', 'featured']
tags = ['webapp', 'research', 'single', 'release']
years = ['2021']
+++

<!--more-->

Telematic awakening: Participating in the 2019 Chilean uprising through a live gestural interface. 26th International Symposium on Electronic Art. Montréal, QC. 

ABSTRACT

The _Telematic awakening_ project was a way of participating in the 2019 Chilean uprising from abroad. I collected interviews and field recordings of the manifestations posted from social media feeds. The recordings were split into sound snippets, sound features are computed, and dimensionality reduction was performed so that the sounds were mapped into a bidimensional performative space. I used a motion tracker device and a machine learning system to capture and map hand positions into the sound space. Sound snippets in this space were concatenated in real time. The interface allowed me to participate telematically in the manifestations by creating layers of other people’s sounds on top of rhythmic and intense music as if I were fighting in the streets.

MOTIVATION

Tens of thousands have been taking to the streets in Chile since last October. People protest against inequality, increased cost of living, privatization of health and education, miserable pensions, and state repression. The unrest was triggered by student-led protests against a metro fare hike. Violence erupted after police fired teargas and water cannon at demonstrators. Some protesters responded by throwing petrol bombs. 

{{<figure src="/img/papers/telematic-manifestation-1.jpg" alt="Large manifestation">}}

State of emergency and curfew were declared. Army and tanks were sent to the streets in most of the country. In response, the protests broadened into a nationwide uprising and turned increasingly violent. The Chilean government announced a series of social reforms to appease the unrest but protesters say the reforms fall short. Dozens of people have died and more than 10,000 people have been arrested since the unrest began. 


{{<figure src="/img/papers/telematic-manifestation-2.jpg" alt="Police brutality">}}

I have been witnessing the uprising from abroad the country but have been pretty much hooked to what is going on and wanting to participate and fight for our rights.


SOUND CORPUS

I was  witnessing the uprising from abroad the country. As a way of participating in the demonstrations I have collected sound recordings from videos posted through social media. 

**Field Recordings**. A number of sounds can be heard in the demonstrations. Most people protest from their own homes making noise by banging pots and pans in order to call for attention in a pacific manner. Protesters sing chants and shout slogans when attending manifestations in the streets. Police react by firing water cannons, teargas, and rubber bullets. The most violent protesters also make barricades to stop police. Some of these barricades have created massive fires. Sirens from police trucks and fire engines are com-monplace in the manifestations.

**Historical Recordings**. I have also collected some of the interviews of Salvador Allende, the first socialist president in the world that arrived to power by democratic means in 1970. Most of his memories have been erased after the coup d'État led by Pinochet in 1973 and his dictatorship until 1990. The lucidity of the interviews and message seem completely pertinent to the current state of affairs, almost 50 years after they were made.




LIVE INTERFACE

For _Telematic awakening_, I play with the two sound corpora in a different fashion. While the field recordings are split into sound snippets of a specific short length, so that when looped they are synchronized to the tempo of the piece; the histor-ical recordings are split by phrase, so that the message they convey is always understood. Hand positions and gestures are acquired and mapped to the sound corpora. At perfor-mance time, I adjust the position of hands using acoustic feedback to play sounds of the same, or different, type.

{{<video autoplay="0" loop="false" src="/videos/audiostellar.mp4" >}}
Hundreds of sound snippets are distributed in a two-dimensional space after dimensionality reduction using t-sne clustering.


Hand positions and gestures are acquired by the Leap Motion hand tracking device and Open Sound Control messages outputted by this device are parsed and rerouted us-ing Max/MSP. The Wekinator, an application for real-time supervised machine learning interaction, is used to learn gestures and positions and map them to specific zones in AudioStellar sound space.

{{<figure src="/img/papers/telematic-diagram.jpg" alt="Schematic of mapping hand gestures into sound corpus">}}
The image shows a high-level diagram of the mapping between sound gestures and the two sound corpora.

PERFORMANCE


{{<youtube YXoA0hHQzEY>}}
I put together the sound corpora and the tools to interact with it in the making of a musical work that I named _Telematic awakening_. 

I premiered the track live at the 2020 MUTEK Festival in Montréal.