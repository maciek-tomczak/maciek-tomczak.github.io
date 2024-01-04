---
layout: page
date: 2020-07-01
title: Drum Synthesis and Rhythmic Transformation with Adversarial Autoencoders
tags: [redrumming, ML]
description: Audio examples accompanying paper for ACM International Conference on Multimedia (ACM MM) 2020.
categories: 
---


**[Tomczak, M.](https://maciek-tomczak.github.io/), [M., Goto](https://staff.aist.go.jp/m.goto/), [J., Hockman](https://www.schoolofdigitalarts.mmu.ac.uk/staff/jason-hockman/), [Drum Synthesis and Rhythmic Transformation with Adversarial Autoencoders, Proceedings of the 28th ACM International Conference on Multimedia (ACM MM), Seattle, WA, USA, October 12–16, 2020.](https://doi.org/10.1145/3394171.3413519)** |

Work conducted during an internship at [Media Interaction Group](https://staff.aist.go.jp/m.goto/MIG/index-j.html), National Institute of Advanced Industrial Science and Technology (AIST), Tsukuba, Japan.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/6aXRdDeihIc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

### 1. Audio synthesis with trained generator (G)

We demonstrate reconstruction of bar-length drum patterns from the generator model trained on real drum recordings. Examples at 22.05kHz sample rate are recreated with Griffin-Lim algorithm together with their corresponding output from the proposed AAE-GM model. More detailed information about data used here can be viewed in Section 3.1 of the [paper](https://doi.org/10.1145/3394171.3413519).

<figure>
    <figcaption><b>Source</b></figcaption>
		{% include audio.html path="assets/audio/ACM20_audio/0092/source_GL-0092_392.mp3" controls=true %}
	<figcaption><b>Output Reconstruction</b></figcaption>
		{% include audio.html path="assets/audio/ACM20_audio/0092/0092_392.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Source</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026/source_GL-0026_64.mp3" controls=true %}
	<figcaption><b>Output Reconstruction</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026/0026_64.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Source</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0070/source_GL-0070_862.mp3" controls=true %}
	<figcaption><b>Output Reconstruction</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0070/0070_862.mp3" controls=true %}
</figure>

### 2. Latent Space Interpolation

<figure>
    {% include figure.html path="assets/audio/ACM20_audio/interp_b.png" class="img-fluid rounded z-depth-1" zoomable=true %}
<figcaption><b>Figure: Interpolation between two rhythmic patterns from source to target</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/16-interp-short.mp3" controls=true %}
</figure>

The proposed model performs rhythmic transformation of bar-length drum patterns as follows:

- Generator reconstruction of **source input**
- Transformation into an **intermediate rhythmic pattern**
- Resulting **output transformation**

A user is given the freedom to manipulate the structure within a bar without reliance on discrete identification of rhythmic boundaries towards a continuous transformation.

- Interpolations in the latent space allow for the mixing of two different drum patterns
- A gradual change is achievable from the **source** rhythmic pattern to the **target** pattern
- The **intermediate latent codes** are produced using a linear interpolation between **source** and **target** latent codes

<figure>
    <figcaption><b>Source Recording</b></figcaption>
        {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/source_GL-0026_64.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Stage 1 | α = 0.0</b></figcaption>
<figcaption><b>Source reconstructed with generator G (not interpolated)</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/interp0_alpha0.0.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Stage 2 | α = 0.25</b></figcaption>
<figcaption><b>This example is similar to source, but begins to be transformed closer to target</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/interp1_alpha0.25.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Stage 3 | α = 0.5</b></figcaption>
<figcaption><b>This example is just in-between the source and the target pattern</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/interp2_alpha0.5.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Stage 4 | α = 0.75</b></figcaption>
<figcaption><b>This example begins to be more rhythmically similar to the target pattern</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/interp3_alpha0.75.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Stage 5 | α = 1.0</b></figcaption>
<figcaption><b>Target reconstructed with generator G (not interpolated)</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/interp4_alpha1.0.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Target Recording</b></figcaption>
    {% include audio.html path="assets/audio/ACM20_audio/0026_to_0012/target_GL-0012_1611.mp3" controls=true %}
</figure>
