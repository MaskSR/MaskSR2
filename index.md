# Full-band General Audio Synthesis With Score-Based Diffusion

This is the demonstration page of the paper "Full-band General Audio Synthesis With Score-Based Diffusion" with some selected samples generated with the proposed method.


## Info

### Abstract

Recent works have shown the capability of deep generative models to tackle general audio synthesis from a single label, producing a variety of impulsive, tonal, and environmental sounds. Such models operate on band-limited signals and, as a result of an autoregressive approach, they are typically conformed by pre-trained latent encoders and/or several cascaded modules. In this work, we propose a diffusion-based generative model for general audio synthesis, named DAG, which deals with full-band signals end-to-end in the waveform domain. Results show the superiority of DAG over
existing label-conditioned generators in terms of both quality and diversity. More specifically, when compared to the state of the art, the band-limited and full-band versions of DAG achieve relative improvements that go up to 40 and 65%, respectively. We believe DAG is flexible enough to accommodate different conditioning schemas while providing good quality synthesis.

### Reference

S. Pascual, G. Bhattacharya., C. Yeh, J. Pons, & J. Serrà.  (2022). **Full-band General Audio Synthesis With Score-Based Diffusion**.

## UrbandSound8K Examples

The following examples are generated using the classifier-free guidance weight gamma=2

### Air conditioner

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_1.wav">
  </audio>
</html>

### Car horn

<html>
  <audio controls>
    <source src="dag_audio/carhorn_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/carhorn_1.wav">
  </audio>
</html>

### Children playing

<html>
  <audio controls>
    <source src="dag_audio/children_playing_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/children_playing_1.wav">
  </audio>
</html>

### Dog bark

<html>
  <audio controls>
    <source src="dag_audio/dogbark_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/dogbark_1.wav">
  </audio>
</html>

### Drilling

<html>
  <audio controls>
    <source src="dag_audio/drilling_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/drilling_1.wav">
  </audio>
</html>

### Engine idling

<html>
  <audio controls>
    <source src="dag_audio/engine_idling_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/engine_idling_1.wav">
  </audio>
</html>

### Gunshot

<html>
  <audio controls>
    <source src="dag_audio/gunshot_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/gunshot_1.wav">
  </audio>
</html>

### Jackhammer

<html>
  <audio controls>
    <source src="dag_audio/jackhammer_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/jackhammer_1.wav">
  </audio>
</html>

### Siren

<html>
  <audio controls>
    <source src="dag_audio/siren_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/siren_1.wav">
  </audio>
</html>

### Street music

<html>
  <audio controls>
    <source src="dag_audio/street_music_0.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/street_music_1.wav">
  </audio>
</html>

## Showcase Examples

The following examples are generated using the classifier-free guidance weight gamma=0

### Wave

**wave splashing**
<html>
  <audio controls>
    <source src="dag_audio/waves_0.wav">
  </audio>
</html>

**wave lapping**
<html>
  <audio controls>
    <source src="dag_audio/waves_1.wav">
  </audio>
</html>

### Wind

**wind whistling**
<html>
  <audio controls>
    <source src="dag_audio/wind_0.wav">
  </audio>
</html>

**wind gust**
<html>
  <audio controls>
    <source src="dag_audio/wind_1.wav">
  </audio>
</html>

### Rain

**rain on grass**
<html>
  <audio controls>
    <source src="dag_audio/rain_0.wav">
  </audio>
</html>

**rain on umbrella**
<html>
  <audio controls>
    <source src="dag_audio/rain_1.wav">
  </audio>
</html>

### River

**close water running**
<html>
  <audio controls>
    <source src="dag_audio/river_0.wav">
  </audio>
</html>

**stream with birds singing**
<html>
  <audio controls>
    <source src="dag_audio/river_1.wav">
  </audio>
</html>

### Fire

**fire embers**
<html>
  <audio controls>
    <source src="dag_audio/fire_0.wav">
  </audio>
</html>

**wood fire crackling**
<html>
  <audio controls>
    <source src="dag_audio/fire_1.wav">
  </audio>
</html>

### Horse

**horse gallop**
<html>
  <audio controls>
    <source src="dag_audio/horse_0.wav">
  </audio>
</html>

**horse carriage**
<html>
  <audio controls>
    <source src="dag_audio/horse_1.wav">
  </audio>
</html>

### Piano

**large dynamics betwen notes**
<html>
  <audio controls>
    <source src="dag_audio/piano_0.wav">
  </audio>
</html>

**soft and reverberant**
<html>
  <audio controls>
    <source src="dag_audio/piano_1.wav">
  </audio>
</html>

### Applause

**crowd applausing and cheering**
<html>
  <audio controls>
    <source src="dag_audio/applause_0.wav">
  </audio>
</html>

**close applausing**
<html>
  <audio controls>
    <source src="dag_audio/applause_1.wav">
  </audio>
</html>

### Footstep

**footsteps on wooden floor**
<html>
  <audio controls>
    <source src="dag_audio/steps_0.wav">
  </audio>
</html>

**walking on grass**
<html>
  <audio controls>
    <source src="dag_audio/steps_1.wav">
  </audio>
</html>

## Style Transfer Examples

We use samples from Medley-solos-DB [1] as "input" (inject it before the first sampling step) to DAG and generate "outputs" with different models.

### Flute

**input**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_flute.wav">
  </audio>
</html>

**output generated by piano model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_flute_to_piano.wav">
  </audio>
</html>


### Trumpet

**input**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_trumpet.wav">
  </audio>
</html>

**output generated by carhorn model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_trumpet_to_carhorn.wav">
  </audio>
</html>

### Singing

**input**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_sing.wav">
  </audio>
</html>

**output generated by piano model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_sing_to_piano.wav">
  </audio>
</html>

**output generated by dog bark model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_sing_to_dogs.wav">
  </audio>
</html>

### Violin

**input**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_violin.wav">
  </audio>
</html>

**output generated by piano model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_violin_to_piano.wav">
  </audio>
</html>

**output generated by dog bark model**
<html>
  <audio controls>
    <source src="dag_conversion/msolo_violin_to_dogs.wav">
  </audio>
</html>


[1] V. Lostanlen, C.E. Cella. Deep convolutional networks on the pitch spiral for musical instrument recognition. Proceedings of the International Society for Music Information Retrieval Conference (ISMIR), 2016.
