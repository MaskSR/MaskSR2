
# MaskSR: Masked Language Model for Full-band Speech Restoration

This is the demonstration page of the paper "MaskSR: Masked Language Model for Full-band Speech Restoration" with some selected samples generated with the proposed method.


## Info

### Abstract

Speech restoration aims at restoring high quality speech in the presence of a diverse set of distortions. Although several deep learning paradigms have been studied for this task,
the power of the recently emerging language models has not been fully explored. In this paper, we propose MaskSR, a masked language model capable of restoring full-band 44.1 kHz speech
jointly considering noise, reverb, clipping, and low bandwidth. MaskSR works with discrete acoustic tokens extracted using a pre-trained neural codec. During training, MaskSR is
optimized to predict randomly masked tokens extracted from the high quality target speech, conditioned on the corrupted speech with various distortions. During inference, MaskSR
reconstructs the target speech tokens with efficient iterative sampling. Extensive experiments show that MaskSR obtains competitive results on both the full-band speech restoration task
and also on sub-tasks compared with a wide range of models.


## Demos

Below, we include audio samples demonstrating how MaskSR performs on the full-band speech restoration task and several sub-tasks.

### General Speech Restoration (ALL-GSR)

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-M</th>
      <th>VoiceFixer</th> 
      <th>NSNet2</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>  
    </tr>
    <tr>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>
      <td><html><audio controls><source src="dag_audio/air_conditioner_0.wav"></audio></html></td>    
    </tr>    
  </tbody>
</table>

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_0.wav">
    <source src="dag_audio/air_conditioner_1.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_1.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_1.wav">
  </audio>
</html>

<html>
  <audio controls>
    <source src="dag_audio/air_conditioner_1.wav">
  </audio>
</html>

