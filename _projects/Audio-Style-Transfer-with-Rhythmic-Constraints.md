---
layout: page
title: Audio Style Transfer with Rhythmic Constraints
description: Results supplementing the paper for the International Conference on Digital Audio Effects (DAFx) 2018.
img: 
importance: 1
category: work
related_publications: 
---


**[Tomczak, M.](https://maciek-tomczak.github.io/), [C., Southall](https://scholar.google.co.uk/citations?user=BrvdPboAAAAJ&hl=en), [J., Hockman](https://www.schoolofdigitalarts.mmu.ac.uk/staff/jason-hockman/), [Audio Style Transfer with Rhythmic Constraints, Proceedings of the 21st International Conference on Digital Audio Effects (DAFx), Aveiro, Portugal, September 4–8, 2018.](https://ant-s4.unibw-hamburg.de/dafx/paper-archive/2018/papers/DAFx2018_paper_48.pdf)** |

### Audio examples

The presented 15 transformation pairs were tested with 3 different loss terms L1, L2 and L3 defined in the [paper](https://ant-s4.unibw-hamburg.de/dafx/paper-archive/2018/papers/DAFx2018_paper_48.pdf), as well as, several additional audio style transfer (AST) transformations. In addition, transformations acquired with default parameters from AST approaches by Barry et al. (2018), Mital (2017) and Ulyanov et al. (2016) are included with the results. Inputs A and B refer to terms <i>content</i> and <i>style</i> used by the authors of the compared papers.

Mashup transformations using L2.


<center>
<figure>
	<figcaption><b>Input A</b>: Marching In The Streets by Harvey Mason</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/samples/Harvey_Mason_Marching_In_The_Streets.mp3" controls=true %}
	<figcaption><b>Input B</b>: Night and Day by Idris Muhammad with George Coleman</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/samples/Idris_Muhammad_with_George_Coleman_Night_and_Day.mp3" controls=true %}
	<figcaption><b>Output Loss 2</b> (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/jazz/Harvey_Mason_Marching_In_The_StreetsIdris_Muhammad_with_George_Coleman_Night_and_Day_1_exp1_fullnorm.mp3" controls=true %}
</figure>
</center>

---

<center>
<figure>
	<figcaption><b>Input A</b>: Colours of the Season by Daudi Matsiko, Yung Veerp, Fazerdaze and others</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/samples/colours_of_the_season.mp3" controls=true %}
	<figcaption><b>Input B</b>: Loop Trigger by Mathew Jonson, GPU Panic</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/samples/loop_trigger.mp3" controls=true %}
	<figcaption><b>Output Loss 2</b> - Loop Triggered Colours of the Season</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/loop_triggered_colors_of_the_season.mp3" controls=true %}
</figure>
</center>


---

Transformation comparisons.

<center>
<h3> Pair 1 </h3>
<figure>
	<figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_ep_02mason_br_02_3_exp3_fullnorm05.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_ep_02mason_br_02_3_exp3_fullnorm05.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_ep_02mason_br_02_3_exp3_fullnorm05.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_ep_02mason_br_02_3_exp3_fullnorm05.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_ep_02mason_br_02_3_exp3_fullnorm05.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_ep_02mason_br_02_3_exp3_fullnorm04.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_ep_02mason_br_02_3_exp3_fullnorm04.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_ep_02mason_br_02_3_exp3_fullnorm04.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 2 </h3>
<figure>
<figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_gs_02mason_cl_03_8_exp8_fullnorm08.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_gs_02mason_cl_03_8_exp8_fullnorm08.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_gs_02mason_cl_03_8_exp8_fullnorm08.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_gs_02mason_cl_03_8_exp8_fullnorm08.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_gs_02mason_cl_03_8_exp8_fullnorm08.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_gs_02mason_cl_03_8_exp8_fullnorm07.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_gs_02mason_cl_03_8_exp8_fullnorm07.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_gs_02mason_cl_03_8_exp8_fullnorm07.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 3 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_hp_02mason_cl_01_10_exp10_fullnorm10.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_hp_02mason_cl_01_10_exp10_fullnorm10.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_hp_02mason_cl_01_10_exp10_fullnorm10.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_hp_02mason_cl_01_10_exp10_fullnorm10.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_hp_02mason_cl_01_10_exp10_fullnorm10.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_hp_02mason_cl_01_10_exp10_fullnorm09.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_hp_02mason_cl_01_10_exp10_fullnorm09.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_hp_02mason_cl_01_10_exp10_fullnorm09.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 4 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_mt_03mason_br_01_12_exp12_fullnorm13.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_mt_03mason_br_01_12_exp12_fullnorm13.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_mt_03mason_br_01_12_exp12_fullnorm13.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_mt_03mason_br_01_12_exp12_fullnorm13.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_mt_03mason_br_01_12_exp12_fullnorm13.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_mt_03mason_br_01_12_exp12_fullnorm12.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_mt_03mason_br_01_12_exp12_fullnorm12.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_mt_03mason_br_01_12_exp12_fullnorm12.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 5 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 6 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/mason_br_03mason_km_03_13_exp13_fullnorm15.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/mason_br_03mason_km_03_13_exp13_fullnorm15.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/mason_br_03mason_km_03_13_exp13_fullnorm15.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/mason_br_03mason_km_03_13_exp13_fullnorm15.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/mason_br_03mason_km_03_13_exp13_fullnorm15.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/mason_br_03mason_km_03_13_exp13_fullnorm14.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/mason_br_03mason_km_03_13_exp13_fullnorm14.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/mason_br_03mason_km_03_13_exp13_fullnorm14.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 7 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/mason_e_03kyle_ob_03_14_exp14_fullnorm16.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/mason_e_03kyle_ob_03_14_exp14_fullnorm16.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/mason_e_03kyle_ob_03_14_exp14_fullnorm16.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/mason_e_03kyle_ob_03_14_exp14_fullnorm16.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/mason_e_03kyle_ob_03_14_exp14_fullnorm16.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/mason_e_03kyle_ob_03_14_exp14_fullnorm15.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/mason_e_03kyle_ob_03_14_exp14_fullnorm15.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/mason_e_03kyle_ob_03_14_exp14_fullnorm15.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 8 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm04.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm04.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm04.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm04.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm04.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm03.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm03.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_ctp_02kyle_nk_03_1_exp1_fullnorm03.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 9 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_ep_01kyle_ob_02_2_exp2_fullnorm02.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_ep_01kyle_ob_02_2_exp2_fullnorm02.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_ep_01kyle_ob_02_2_exp2_fullnorm02.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_ep_01kyle_ob_02_2_exp2_fullnorm02.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_ep_01kyle_ob_02_2_exp2_fullnorm02.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_ep_01kyle_ob_02_exp2_fullnorm01.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_ep_01kyle_ob_02_exp2_fullnorm01.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_ep_01kyle_ob_02_exp2_fullnorm01.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 10 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_ep_03kyle_hp_03_5_exp5_fullnorm06.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_ep_03kyle_hp_03_5_exp5_fullnorm06.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_ep_03kyle_hp_03_5_exp5_fullnorm06.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_ep_03kyle_hp_03_5_exp5_fullnorm06.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_ep_03kyle_hp_03_5_exp5_fullnorm06.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_ep_03kyle_hp_03_5_exp5_fullnorm05.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_ep_03kyle_hp_03_5_exp5_fullnorm05.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_ep_03kyle_hp_03_5_exp5_fullnorm05.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 11 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_gs_01mason_km_02_6_exp6_fullnorm07.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_gs_01mason_km_02_6_exp6_fullnorm07.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_gs_01mason_km_02_6_exp6_fullnorm07.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_gs_01mason_km_02_6_exp6_fullnorm07.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_gs_01mason_km_02_6_exp6_fullnorm07.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_gs_01mason_km_02_6_exp6_fullnorm06.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_gs_01mason_km_02_6_exp6_fullnorm06.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_gs_01mason_km_02_6_exp6_fullnorm06.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 12 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_gs_03mason_e_02_9_exp9_fullnorm09.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_gs_03mason_e_02_9_exp9_fullnorm09.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_gs_03mason_e_02_9_exp9_fullnorm09.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_gs_03mason_e_02_9_exp9_fullnorm09.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_gs_03mason_e_02_9_exp9_fullnorm09.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_gs_03mason_e_02_9_exp9_fullnorm08.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_gs_03mason_e_02_9_exp9_fullnorm08.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_gs_03mason_e_02_9_exp9_fullnorm08.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 13 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm03.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm03.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm03.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm03.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm03.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm02.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm02.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_ctp_01kyle_nk_02_0_exp0_fullnorm02.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 14 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_mt_01mason_km_01_7_exp7_fullnorm11.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_mt_01mason_km_01_7_exp7_fullnorm11.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_mt_01mason_km_01_7_exp7_fullnorm11.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_mt_01mason_km_01_7_exp7_fullnorm11.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_mt_01mason_km_01_7_exp7_fullnorm11.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_mt_01mason_km_01_7_exp7_fullnorm10.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_mt_01mason_km_01_7_exp7_fullnorm10.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_mt_01mason_km_01_7_exp7_fullnorm10.mp3" controls=true %}
</figure>
</center>

---

<center>
<h3> Pair 15 </h3>
<figure>
    <figcaption>Input A</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputA/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Input B</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/inputB/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 1 (Vanilla AST - Content A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L1/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 2 (Mashup - Style A + Style B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L2/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Loss 3 (Augmented Mashup - Style A + Style B + Content B)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/results/L3/out/kyle_nk_01kyle_hp_01_4_exp4_fullnorm14.mp3" controls=true %}
	<figcaption>Vanilla AST (Barry 2018)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/barry/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
	<figcaption>Vanilla AST (Mital 2017)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/mital/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
	<figcaption>Vanilla AST (Ulyanov 2016)</figcaption>
		{% include audio.html path="assets/audio/DAFx18_audio/ulyanov/mp3/kyle_nk_01kyle_hp_01_4_exp4_fullnorm13.mp3" controls=true %}
</figure>
</center>

---

### References:

1. Shaun Barry and Youngmoo Kim, “Style transfer for musical audio using multiple time-frequency representations,” 2018, Available at: <a href="https://github.com/pkmital/time-domain-neural-audio-style-transfer">https://github.com/anonymousiclr2018/Style-Transfer-for-Musical-Audio</a>.

2. Parag K. Mital, “Time domain neural audio style transfer,” 2017, Available at: <a href="https://github.com/pkmital/time-domain-neural-audio-style-transfer">https://github.com/pkmital/time-domain-neural-audio-style-transfer</a>.

3. Dmitry Ulyanov and Vadim Lebedev, “Audio texture synthesis and style transfer,” 2016, Available at: <a href="https://github.com/pkmital/time-domain-neural-audio-style-transfer">https://dmitryulyanov.github.io/audio-texture-synthesis-and-style-transfer/</a>.
