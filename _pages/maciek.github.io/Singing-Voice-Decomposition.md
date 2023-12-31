---
layout: page
date: "2020-07-01"
permalink: /maciek.github.io/Singing-Voice-Decomposition
title: Singing Voice Decomposition
date: "2021-09-14"
tags: [ML]
description: "Audio examples accompanying an unpublished paper titled Investigating Information Bottleneck in Variational Autoencoder-based Singing Voice Decomposition which I worked on with Kin Wah Edward Lin (AIST), Tomoyasu Nakano (AIST), Jason Hockman (BCU), and Masataka Goto (AIST)"
nav: false
---

# Abstract
> We investigate how the size of latent variables, functioning as an information bottleneck, affects the reconstruction and disentanglement quality in variational autoencoder (VAE)-based singing voice decomposition. Evaluating a large number of latent variable sizes is impractical due to computational costs. To make this investigation feasible, we first design a VAE that is quick in training and generation and remains stable during training. We then assess the control exerted by different latent variable sizes within our model. For reconstruction quality quantification, we calculate log-spectrogram differences and short-time objective intelligibility (STOI) scores between the ground truth and reconstructed signals. To evaluate disentanglement quality, we train classifiers for each latent variable size to measure the encoded information about generative factors. Our tests on two singing voice datasets, the publicly available NUS English dataset and the newly compiled JP Japanese singing experience database, revealed consistent trends in the impact of latent variable size across both datasets. This suggests the reliability of our results and highlights a trade-off between reconstruction and disentanglement quality. These findings offer insights into the voice conversion capabilities of VAEs and suggest directions for improving VAE-based singing voice decomposition.

# System Overview
<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="_pages/maciek.github.io/singing-voice/arch_horizon.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>
<b>Figure 1:</b> Singing voice decomposition overview with encoders $$E_{\rho}$$ and $$E_{c}$$ representing low-level information for pitch $$Z_{\rho}$$ (orange) and content $$Z_{c}$$ (pink) and singer style (i.e., singer ID) $$Z_{\psi}$$ (blue). The encoded pitch, content and style information are concatenated onto one latent variable $$z$$. The generator $$G$$ (yellow) outputs a single log-spectrogram frame. All frames are concatenated together to produce a singing performance. The system is capable of synthesising full singing performances due to dilated CNN architecture.

# Listening Examples
While listening to the following audio examples, please note that some sonic artifacts are present here and also in other state-of-the-art singing voice conversion methods (e.g., [[1]](#ref)). The reduction of such artifacts is not the main target of our research and will be tackled by a research community in the future. Please focus on listening to the conversion of musical characteristics such as timbre and singing style. 

Please allow a moment if the audio does not load immediately after pressing play.

## AIST-SEDB-120JP database - Female (Song 13 & ID 27)

Each presented audio example follows song and singer IDs in Tables I and II in the paper. All examples are 16-bit 22050 Hz WAV files.

<figure>
<figcaption><b>Ground truth (female)</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A_SOURCE_female_JP.mp3" controls=true %}
</figure>


<figure>
<figcaption><b>Reconstruction (female)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A_Z4_RECON_female_JP.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; female)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A4_Z4_female_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A3_Z4_female_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A2_Z4_female_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A1_Z4_female_female_JP.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; male)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A4_Z4_female_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A3_Z4_female_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A2_Z4_female_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A1_Z4_female_male_JP.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; male)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 100</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_JP/A1_Z100_female_male_JP.mp3" controls=true %}
<figcaption>Example sounds almost the same as the ground truth with <b>no voice conversion</b></figcaption>
</figure>

## AIST-SEDB-120JP database - Male (Song 56 & ID 04)

Each presented audio example follows song and singer IDs in Tables I and II in the paper. All examples are 16-bit 22050 Hz WAV files.

<figure>
<figcaption><b>Ground truth (male)</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A_SOURCE_male_JP.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Reconstruction (male)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A_Z4_RECON_male_JP.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; female)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A4_Z4_male_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A3_Z4_male_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A2_Z4_male_female_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A1_Z4_male_female_JP.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; male)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A1_Z4_male_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A3_Z4_male_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A2_Z4_male_male_JP.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A4_Z4_male_male_JP.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; female)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 100</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_JP/A4_Z100_male_female_JP.mp3" controls=true %}
<figcaption>Example sounds almost the same as the ground truth with <b>no voice conversion</b></figcaption>
</figure>

## NUS-48E database - Female (Song 18 & ID ADIZ)

Each presented audio example follows song and singer IDs in the original NUS-48E database [[2]](#ref). All examples are 16-bit 22050 Hz WAV files.

<figure>
<figcaption><b>Ground truth (female)</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A_SOURCE_female_EN.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Reconstruction (female)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A_Z4_RECON_female_EN.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; female)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A4_Z4_female_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A3_Z4_female_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A2_Z4_female_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A1_Z4_female_female_EN.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; male)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A4_Z4_female_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A3_Z4_female_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A2_Z4_female_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A1_Z4_female_male_EN.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (female &rarr; male)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 100</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_female_EN/A1_Z100_female_male_EN.mp3" controls=true %}
<figcaption>Example sounds almost the same as the ground truth with <b>no voice conversion</b></figcaption>
</figure>

## NUS-48E Database - Male (Song 15 & ID JLEE)

Each presented audio example follows song and singer IDs in the original NUS-48E database [[2]](#ref). All examples are 16-bit 22050 Hz WAV files.

<figure>
<figcaption><b>Ground truth (male)</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A_SOURCE_male_EN.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Reconstruction (male)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A_Z4_RECON_male_EN.mp3" controls=true %}
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; female)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A4_Z4_male_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A3_Z4_male_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A2_Z4_male_female_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A1_Z4_male_female_EN.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; male)</b></figcaption>
<figcaption>4 examples generated with a trained model using space <b>Zc = 4</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A1_Z4_male_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A3_Z4_male_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A2_Z4_male_male_EN.mp3" controls=true %}
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A4_Z4_male_male_EN.mp3" controls=true %}
	<figcaption>Above examples show varied timbres and successful conversions to different singers</figcaption>
</figure>

<figure>
<figcaption><b>Voice Conversion (male &rarr; female)</b></figcaption>
<figcaption>Generator trained using space <b>Zc = 100</b></figcaption>
    {% include audio.html path="_pages/maciek.github.io/singing-voice/A_male_EN/A4_Z100_male_female_EN.mp3" controls=true %}
<figcaption>Example sounds almost the same as the ground truth with <b>no voice conversion</b></figcaption>
</figure>

# <a name="ref">References</a>


[1] [Yin-Jyun Luo et al. “Singing voice conversion with disentangled representations of singer and vocal technique using variational autoencoders”. In: IEEE international conference on acoustics, speech and signal processing (ICASSP). 2020.](https://ismir19-217.github.io/icassp20-audio-sample/)


[2] [Zhiyan Duan et al. “The NUS sung and spoken lyrics corpus: a quantitative comparison of singing and speech”. In: IEEE Asia-pacific signal and informationprocessing association annual summit and conference (APSIPA ASC). 2013.](https://smcnus.comp.nus.edu.sg/nus-48e-sung-and-spoken-lyrics-corpus/)
