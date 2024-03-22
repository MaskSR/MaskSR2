
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
      <td><html><audio controls><source src="GSR/Unprocessed/1_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/1_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/1_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/1_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/1_simulated.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/2_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/2_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/2_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/2_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/2_simulated.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/3_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/3_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/3_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/3_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/3_simulated.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/4_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/4_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/4_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/4_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/4_simulated.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/5_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/5_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/5_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/5_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/5_simulated.wav"></audio></html></td>  
    </tr>  
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/6_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/6_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/6_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/6_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/6_simulated.wav"></audio></html></td>  
    </tr>    
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/7_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/7_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/7_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/7_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/7_simulated.wav"></audio></html></td>  
    </tr> 
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/8_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/8_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/8_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/8_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/8_simulated.wav"></audio></html></td>  
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/9_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/9_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/9_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/9_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/9_simulated.wav"></audio></html></td>  
    </tr>    
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/10_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/10_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/MaskSR-M/10_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/10_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/NSNet2/10_simulated.wav"></audio></html></td>  
    </tr>                     
  </tbody>
</table>

### Speech Super Resolution (SR)

#### From 2kHz to 44.1kHz

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
  </tbody>
</table>

#### From 4kHz to 44.1kHz

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
  </tbody>
</table>

#### From 8kHz to 44.1kHz

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
  </tbody>
</table>


### DNS-2020 no_reverb

#### no_reverb test samples

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>MaskSR-M</th>
      <th>FRCRN</th> 
      <th>DEMUCS</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
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
    </tr>
  </tbody>
</table>

#### with_reverb test samples

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>MaskSR-M</th>
      <th>FRCRN</th> 
      <th>DEMUCS</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
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
    </tr>
  </tbody>
</table>

#### real_recordings test samples

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>MaskSR-M</th>
      <th>FRCRN</th> 
      <th>DEMUCS</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
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
    </tr>
  </tbody>
</table>

