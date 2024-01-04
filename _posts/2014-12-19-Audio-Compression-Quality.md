---
layout: page
title: Audio Compression Quality
date: 2014-12-19
tags: [lossy-compression,MP3,listening-tests]
description: On what's left out when compressing to MP3.
categories: 
---


I wrote the following article back when I was an undergrad finishing my first year at Birmingham City University in 2013. Coincidentally, to my surprise the same experiment I describe here was given to me in class by my DSP professor Ian Williams a few weeks after I published this. Anyway, after revisiting these tests more recently I can sum them up with the good ol' <em>it depends</em> :)

**TL;DR** A 320kbps VBR Mp3 can be enough but it depends to what you are listening to and what system you are listening that on.

Original article is posted [here](https://maciekonsound.wordpress.com/2014/12/19/listening-tests/).

<h2>Listening Tests</h2>
<p style="text-align:left;" align="CENTER">So in the previous <a title="Article on CD Ripping" href="https://maciek-tomczak.github.io/maciek.github.io/Audio-Ripping-and-Compression" target="_blank">article</a> we managed to rip and compress our really good quality Mp3s. So now its right time to ask questions… Just how good are these Mp3s if compared to the sound on a CD? Have we set up the encoder correctly? The most obvious way to find out is to conduct a listening test, but…</p>
But there is a problem.

It turns out that it is quite challenging to compare two audio sources of different quality, timing, and volume. The traditional method of audio listening tests is to play one song followed by another and ask which one sounded better. Interestingly enough, our brains recognize a slight increase in volume as an increase in clarity, which is critical in this situation, as we want to avoid possibility of confirmation bias. We need a way of switching between two audio sources of different quality at any point in a song, with no delays or changes in timing and volume.

I’ve observed many fierce debates in real live and online, where people insisted that they can hear the difference between 320kbps Mp3s and ones of even slightly lower bit rate. Some say that Mp3s are no good enough for 'serious' audio equipment. Let’s hear if this is true.

I ripped one song from the same CD as an uncompressed wave file, as a 320 bit rate Mp3 and as the blend of VBR.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/11.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

I imported the raw wave file and the 320kbps Mp3 into Audacity, one after the other.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/21.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

Since, the Mp3 compression process had padded the start and finish of the file, it is necessary to remove the silence so that both tracks are aligned.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/31.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

It’s quite slow and notorious to align both tracks as audacity does not support a user-friendly zoom in/out option. However, once you managed to zoom in so that you can see all the individual samples, I suggest to pick one that is standing out, and use it as a guide-sample.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/41.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

Now the interesting part kicks in. I selected the whole region of the 320kbps Mp3 and inverted it. It means that whenever the waveform had previously gone up it now is going down, and vice versa.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/51.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

Then I selected the uncompressed wave file with the inverted Mp3, and clicked mix and render.

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/61.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

This action created a mix file that represents the differences between our uncompressed and compressed files. I think it’s really interesting to see this pretty digital representation of the data chunk that we loose completely when compressing our CD files. This is how it sounds like: <audio controls src="./stage1_T1.wav"></audio>

Cool, right? Does it make a difference? :)

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/71.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

Then I imported a 320kbps Mp3 into Audacity. In the screenshot above you can see very clearly (on the same zoom-in setting on both tracks) differences in the sizes of both files. After this, I did the sample alignment again, and hit the play button. Both tracks plated simultaneously and sounded like the source CD. Mathematically, it was the source CD. The difference file and the compressed file equaled the source file. By muting the difference file at any point in the song, I could hear without distortion, or changes in volume, what is the difference in quality after compressing a wave file into a 320kbps Mp3.

I listened, and listened, but there was no difference to be heard. Don’t believe me? See if you can spot the points where the quality changes.

<center>
<figure>
		{% include audio.html path="assets/audio/audio-compression/stage1_T2.mp3" controls=true %}
</figure>
</center>

Did you hear any difference? No? Yes? Maybe? Try it again and listen for an increase in quality at 5 seconds which disappears at 16. Using modern Mp3 encoding methods, a 320 bit rate Mp3 sounds very much like the original (at least to my ears).

<center>
<figure>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/audio/audio-compression/81.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</figure>
</center>

I repeated the same test using a VBR Mp3 instead of the normal 320kbps. As you can see the difference file is smaller from the normal 320 bitrate Mp3. You can listen to it and see if there is any detectable change in playback quality.

<center>
<figure>
		{% include audio.html path="assets/audio/audio-compression/stage2_T3.mp3" controls=true %}
</figure>
</center>

The quality should increase slightly after 5 seconds, then drop off at 16. I cannot hear any difference here as well. So does it mean that the 320kbps MPS sounds as good as an uncompressed CD .wav format?

In order to do a more obvious comparison I did the same test using a 56 bit rate Mp3 and the results were, as expected, humongous. The difference track was huge. You could really see how much audio was lost in compression. The 56 bit rate audio sounded horrible, but as soon as I unmuted the difference track it was suddenly sounding like the CD once again. You can hear it for yourself here.

<center>
<figure>
		{% include audio.html path="assets/audio/audio-compression/stage3_T4.mp3" controls=true %}
</figure>
</center>

In the end, I have to say that it is (almost) impossible to tell the difference between a song as an uncompressed wave file and a song that has been compressed as 320 VBR. I used DT 770s and my M-audio interface for these tests, and of course all results were confirmed using my teenage ears. Furthermore, the 320 VBR file I used wighted 8.2 MB, the normal CBR Mp3 weighted 10.3 MB, and the uncompressed wave weighted 45.4 MB. This shows that the VBR method provides great results while taking 25.6% less space than a normal CBR method in this example.

I think many people are not 100% honest with themselves when they say that all Mp3s sound worse than CDs. This goes especially for people with worn out ears who speak such heresies. On the contrary, I’ve read a few interesting posts where audiophiles argued that the average person doesn’t have the knowledge or experience to verbalize the fact that what they hear is an MP3. I don’t think that is the case in the kind of tests I conducted, as I tried it on few other recordings, and all the findings were the same. However, it may vary in more surgical audio situations where a trained ear, that knows exactly what to look for in the high frequencies, will be able to distinguish between a wave file and Mp3. Often, it will be the 'air' of high frequencies that may provide some small differences between a good quality MP3 and a .wav file.

Speaking of recording, mixing and mastering though... I would never include good quality Mp3 files in my mixes because I believe there are certain situations that ask for certain tools. I’d try to keep my recordings the highest quality possible, but that also may change depending on a final, envisioned version of a song I’ll mix.

Again, Mp3 algorithms improved drastically over the past decade. We do not suffer anymore from tons of audio errors if an Mp3 is ‘only’ 192kbps. In fact, I’m positive that dropping to 128kbps would still be acceptable for many people. Especially if played on poor playback platforms such as iPods, iPods or similar, where listening conditions aren’t great anyways. I think we should admit however, that correctly compressed, high quality Mp3s are good enough to satisfy the needs of serious music listeners. Listeners who strive for a really good quality sounds that can be expressed through some expensive equipment.

I’m also attaching this little section here, as I find it really fascinating how the same file compression comparison test can be shown visually.

So here is an alternative way of looking at compression subject.

<a title="Lossy Audio Codec's Comparison" href="http://www.head-fi.org/t/225356/lossy-audio-codecs-comparison-huge-amount-of-pics-itunes-update-on-p-7" target="_blank">Lossy Audio Codec’s Comparison</a>

Another interesting visual example.

<a title="How to check quality of Mp3 file" href="http://www.walterdevos.be/how-to-check-quality-of-mp3-file" target="_blank">How to check quality of Mp3 file</a>

I’d like to thank <a id="yui-gen18" title="Bugbrain's post on Recordingreview.com" href="http://forum.recordingreview.com/f8/endless-mp3-vs-wav-debate-randomized-blind-listening-test-40661/" target="_blank" rel="nofollow">Bugbrain</a>, <a title="Forum profile" href="http://www.head-fi.org/u/49722/sir-nobax" target="_blank">Nobax</a>, <a title="Walter's blog" href="http://blog.walterdevos.be/" target="_blank">Walter</a>, and <a title="Jax's website" href="http://www.jax184.com/" target="_blank">Jax</a> for inspiring me to conduct this experiment.

Maciek
