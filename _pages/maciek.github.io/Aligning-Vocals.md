---
layout: page
permalink: /maciek.github.io/Aligning-Vocals
title: Aligning Vocals - Drudgery or a Walk in the Park?
date: "2014-12-20"
tags: [vocal-alignment,mixing]
description: On manual and automatic alignment of vocal recordings.
nav: false
---

I wrote the following article back in 2013 and today the problem of aligning things in time is still very close to my heart.

Original article is posted [here](https://maciekonsound.wordpress.com/2014/12/19/aligning-vocals-drudgery-or-a-walk-in-the-park/).

#### Aligning Vocals - Drudgery or a walk in the park?

<div class="entry-content">
This time I want to show you a vocal aligning plugin I’ve recently found and started using like a madman. Knowing that I often work with tracks that I need to have aligned pretty tight, this discovery was just what I needed. When I think of all the long ‘late’ hours spent on aligning vocals in software such as <a href="http://www.celemony.com/en/melodyne/what-is-melodyne" target="_blank">Melodyne</a> I get these uncomfortable chills on my back, ughh. Oh man, why didn’t I know about VocAlign before?! Well there is a good reason for it. I just wasn’t looking for it! To be honest I would be probably still working with software like Melodyne till this day if my friend hadn’t told me about it, but about that in a second. So, I wanted to think that the software just wasn’t around until recently but here came a surprise for me. Apparently the VocAlign project was first released in 2001 and now grew to see its new version which is available <a href="https://www.synchroarts.com/products/vocalign-pro/overview" target="_blank">here</a>.

One day I talked with my friend about timing vocals to one of the songs I was working on and (of course) I’d go on, and on about how annoying working with Melodyne can be. It can very easily destroy the signal making it sound like, hmm, well like Melodyne. Well, from time to time the vocals I work on need to sound alien-like, but hey welcome to the 21st century! Sometimes alien-like vocals may be the thing that the song calls for, right? With many popular songs nowadays you simply cannot tell if the vocals were actually sang by an actual human being.

But back to the story. My friend answered to my complaining with a question ’why don’t you just use VocAlign for your tracks?’. I wasn’t completely aware at the time of how that conversation will change the way I handle vocal aligning. but now, I know, and I am really excited to share some of my results.

So what’s VocAlign? It is an audio plugin that will automatically align two audio signals so that the timing of one matches the other. It works at 16 and 24 bit resolutions and sampling frequencies from 44.1 to 192kHz. But what truly maters is the simplicity and speed of the software. The work that was taking me an hour using Melodyne for example, decreased now to only few minutes. Don’t get me wrong, I still think Melodyne is a great piece of software and I still use it often, but so far VocAlign has made vocal aligning to me be just like a walk in the park.

<strong>Aligning with VocAlign: Examples</strong>

I will present 3 different examples that will consist of: 1) an .mp3 containing just a raw vocal tracks, 2) .mp3 containing vocal VocAligned tracks and 3) the mixed track.

<center>
<figure>
        <div class="caption"> Example 1 No Effects </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_1_NoEffects.mp3" controls=true %}
        <div class="caption"> Example 1 VocAlign </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_1_VocAlign.mp3" controls=true %}
        <div class="caption"> Example 1 Mix </div>
        {% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_1_Mix.mp3" controls=true %}
</figure>
</center>

The differences between not aligned and aligned tracks may be subtle in this example but I wanted to show it anyways because many things mastering engineers do, Are subtle. I learned that from Dave Pensado and his amazing series on YT called <a href="http://www.pensadosplace.tv/" target="_blank">Pensado’s Place</a>. Defnitely worth checking out if you are into music production, sound engineering, mastering, or anything else that has something to do with studio work.

So in this example we will see how VocAlign deals with a bit more recognisable timing variations.
<center>
<figure>
        <div class="caption"> Example 2 No Effects </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_2_NoEffects.mp3" controls=true %}
        <div class="caption"> Example 2 VocAlign </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_2_VocAlign.mp3" controls=true %}
        <div class="caption"> Example 2 Mix </div>
        {% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_2_Mix.mp3" controls=true %}
</figure>
</center>

In this example you can hear the differences much better (if you still can’t hear it then listen out for the word ‘hearts’)

Now I will just quickly write down the process I have to go through to align one track to the other: 1) Open VocAlign, 2) side chain the track I’m working on to the track that I want to align it to, 3) click ‘Capture Audio’, 4) playback the part that I want to align, 5) press ‘Analyse’>’Align’>’Edit’ and voilà, I have my aligned track.

Excluding the playback time the whole process takes me a few seconds. How amazing is that?! Definitely much better than moving each syllable manually.

But of course nothing is perfect (That's a good thing. SMILEY)

<strong>Where does a subtle (=’good’) aligning end and where does a hardcore (=’not so good’) aligning start?</strong>

<center>
<figure>
        <div class="caption"> Example 3 No Effects </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_3_NoEffects.mp3" controls=true %}
        <div class="caption"> Example 3 VocAlign </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_3_VocAlign.mp3" controls=true %}
</figure>
</center>

What was wrong? You can probably tell yourself already.

Well, VocAlign uses sophisticated pattern matching algorithms that compare digital data. VocAlign moves AND stretches our recording so that it creates as closest match as possible to the side chained track. The obvious problem that arrises is this ‘unnaturally-stretchy-signal’ (probably the best way to describe it :)

Do we want it? Maybe yes, maybe not. In the end, I worked my way to have it sound like this:


<center>
<figure>
        <div class="caption"> Example 3 Mix </div>
		{% include audio.html path="_pages/maciek.github.io/aligning-vocals/Example_3_Mix.mp3" controls=true %}
</figure>
</center>


Furthermore, in example 3 you should also notice the word timing differences. These may cause more problems if one is not careful.

<strong>The Bottom Line</strong>
<ul>
	<li>I no longer have to waste my time aligning each syllable of my layered vocals.</li>
	<li>Working with backing vocals has never been easier.</li>
	<li>Yes, VocAlign sometimes does this weird stretchy thing to the signal, but so what?  I’m ready to forgive these little flaws if the process of aligning, as a whole, has been reduced to just a few mouse clicks.</li>
</ul>

I still use both <a href="http://www.celemony.com/en/melodyne/what-is-melodyne" target="_blank">Melodyne by Celemony</a> and <a href="https://www.synchroarts.com/products/vocalign-pro/overview" target="_blank">VocAlign by Synchro Arts</a> and I'm really interested in what the future research holds for automatic vocal alignment and manipulation.

This is the band that I used for the above examples, Make Sure You Check Their YT Channel: <a href="http://www.youtube.com/user/JetfaceGroup" target="_blank" rel="nofollow">JetfaceGroup – YouTube</a>

</div>
<h3></h3>
Maciek
