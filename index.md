
# Joint Semantic Knowledge Distillation and Masked Acoustic Modeling for Full-band Speech Restoration with Improved Intelligibility

Xiaoyu Liu,    Xu Li,    Joan Serrà,    Santiago Pascual

This is the demonstration page of the paper "Joint Semantic Knowledge Distillation and Masked Acoustic Modeling for Full-band Speech Restoration with Improved Intelligibility" with samples generated with the proposed method and some other baseline methods.


## Abstract

Speech restoration aims at restoring full-band speech with
high quality and intelligibility, considering a diverse set of distortions.
MaskSR is a recently proposed generative model for this task. As other
models of its kind, MaskSR attains high quality but, as we show,
intelligibility can be substantially improved. We do so by boosting the
speech encoder component of MaskSR with predictions of semantic
representations of the target speech, using a pre-trained self-supervised teacher model. Then, a masked language model is conditioned on the learned semantic features to predict acoustic tokens that encode low level spectral details of the target speech. We show that, with the same MaskSR model capacity and inference time, the proposed model, MaskSR2, significantly reduces the word error rate, a typical metric for intelligibility. MaskSR2 also achieves competitive word error rate among other models, while providing superior quality. An ablation study shows the effectiveness of various semantic representations.


## Demos

Below, we show audio samples demonstrating how MaskSR2 performs on the full-band speech restoration task and several sub-tasks compared with some baseline methods.

## Full-band 44.1 kHz speech restoration

### Speech restoration with distortions including noise, reverb, clipping, and low bandwidth

#### MaskSR2 vs. MaskSR: Improved Intelligibility

These samples demonstrate that MaskSR2 improves the intelligibility of the generated speech compared with those of MaskSR. The semantic knowledge distillation preserves the phonetic content after removing the distortions.

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>Transcription</th>
      <th>MaskSR-L</th> 
      <th>MaskSR2-L</th>
      <th>Improved words</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/2_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/2_clean.wav"></audio></html></td>
      <th>Throughout the centuries, people have explained the rainbow.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/2_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/2_simulated_proc.wav"></audio></html></td>
      <th>rainbow</th> 
    </tr>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p364_231_910.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p364_231_910.wav"></audio></html></td>
      <th>I could not believe the results.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p364_231_910_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p364_231_910_proc.wav"></audio></html></td>
      <th>I could not believe the results</th> 
    </tr>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/10_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/10_clean.wav"></audio></html></td>
      <th>I have so much respect for him. His friend</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/10_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/10_simulated_proc.wav"></audio></html></td>
      <th>for</th> 
    </tr>  
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p361_174_66.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p361_174_66.wav"></audio></html></td>
      <th>The quality of life is difficult for them.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p361_174_66_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p361_174_66_proc.wav"></audio></html></td>
      <th>life, difficult</th> 
    </tr>    
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p362_158_555.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p362_158_555.wav"></audio></html></td>
      <th>However, the story has a happy ending.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p362_158_555_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p362_158_555_proc.wav"></audio></html></td>
      <th>ending</th> 
    </tr> 
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p364_065_429.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p364_065_429.wav"></audio></html></td>
      <th>It's not going to work.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p364_065_429_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p364_065_429_proc.wav"></audio></html></td>
      <th>it's</th> 
    </tr>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <th>I would not do that.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p360_354_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p360_354_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <th>do</th> 
    </tr>    
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <th>And the other winners are.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <th>other</th> 
    </tr>                                    
  </tbody>
</table>

#### MaskSR2 vs. other full-band models

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/1_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/1_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/1_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/1_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/1_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/1_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/3_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/3_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/3_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/3_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/3_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/3_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/5_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/5_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/5_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/5_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/5_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/5_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/6_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/6_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/6_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/6_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/6_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/6_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/7_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/7_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/7_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/7_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/7_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/7_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/8_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/8_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/8_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/8_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/8_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/8_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/9_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/9_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/9_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/9_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/9_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/9_simulated_proc.wav"></audio></html></td>
    </tr> 
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/11_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/11_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/11_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/11_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/11_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/11_simulated_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/12_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/12_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/12_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/12_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/12_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/12_simulated_proc.wav"></audio></html></td>
    </tr> 
    <tr>
      <td><html><audio controls><source src="GSR/Unprocessed/13_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/Target/13_clean.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/13_simulated_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR2-L/13_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="GSR/VoiceFixer/13_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/13_simulated_proc.wav"></audio></html></td>
    </tr>                                
  </tbody>
</table>

### Bandwidth Extension

#### From 1 kHz to full bandwidth

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>         
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p360_354_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p360_354_mic1_1000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p360_354_mic1_1000_cheby1_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

#### From 2 kHz to full bandwidth

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>     
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p360_275_mic1_2000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p360_275_mic1_2000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p360_275_mic1_2000_cheby1_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p363_037_mic1_2000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p363_037_mic1_2000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p363_037_mic1_2000_cheby1_proc.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

#### From 4 kHz to full bandwidth

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>    
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p361_084_mic1_4000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p361_084_mic1_4000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p361_084_mic1_4000_cheby1_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p364_249_mic1_4000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p364_249_mic1_4000_cheby1_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="SR/VoiceFixer/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p364_249_mic1_4000_cheby1_proc.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

### Declipping

#### Clipping threshold 0.1

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="DECLIP/0.1/noisy/p360_001_mic1_10.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DECLIP/0.1/clean/p360_001_mic1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p360_001_mic1_10.00_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p360_001_mic1_10.00_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DECLIP/0.1/VoiceFixer/p360_001_mic1_10.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p360_001_mic1_10.00_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DECLIP/0.1/noisy/p360_004_mic1_10.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DECLIP/0.1/clean/p360_004_mic1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p360_004_mic1_10.00_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p360_004_mic1_10.00_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DECLIP/0.1/VoiceFixer/p360_004_mic1_10.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p360_004_mic1_10.00_proc.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

#### Clipping threshold 0.25

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>
      <th>VoiceFixer</th>
      <th>DeepFilterNet3</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="DECLIP/0.25/noisy/p361_004_mic1_4.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DECLIP/0.25/clean/p361_004_mic1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p361_004_mic1_4.00_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p361_004_mic1_4.00_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DECLIP/0.25/VoiceFixer/p361_004_mic1_4.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p361_004_mic1_4.00_proc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DECLIP/0.25/noisy/p361_005_mic1_4.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DECLIP/0.25/clean/p361_005_mic1.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/p361_005_mic1_4.00_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/p361_005_mic1_4.00_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DECLIP/0.25/VoiceFixer/p361_005_mic1_4.00.wav"></audio></html></td>
      <td><html><audio controls><source src="DeepFilterNet3/p361_005_mic1_4.00_proc.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

## Wideband 16 kHz speech denoising

### DNS-2020 no_reverb test samples

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>Target</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>      
      <th>FRCRN</th> 
      <th>DEMUCS</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp178_baby_416649_0_snr15_tl-32_fileid_127.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/Target/clean_fileid_127.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR-L/clnsp178_baby_416649_0_snr15_tl-32_fileid_127_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/clnsp178_baby_416649_0_snr15_tl-32_fileid_127_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp178_baby_416649_0_snr15_tl-32_fileid_127.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp178_baby_416649_0_snr15_tl-32_fileid_127.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/Target/clean_fileid_147.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR-L/clnsp25_babble_188218_21_snr5_tl-25_fileid_147_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/clnsp25_babble_188218_21_snr5_tl-25_fileid_147_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/Target/clean_fileid_81.wav"></audio></html></td>      
      <td><html><audio controls><source src="MaskSR-L/clnsp62_birds_413745_6_snr14_tl-33_fileid_81_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/clnsp62_birds_413745_6_snr14_tl-33_fileid_81_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/Target/clean_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/clnsp71_babble_188218_26_snr4_tl-20_fileid_275_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/clnsp71_babble_188218_26_snr4_tl-20_fileid_275_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

### DNS-2020 real_recordings test samples

<table>
  <thead>
    <tr>
      <th>Unprocessed</th>
      <th>MaskSR-L</th>
      <th>MaskSR2-L</th>      
      <th>FRCRN</th> 
      <th>DEMUCS</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/audioset_realrec_airconditioner_8v4sEeK2Owc_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/audioset_realrec_airconditioner_8v4sEeK2Owc_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/audioset_realrec_airconditioner_EK746oGQz6E_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/audioset_realrec_airconditioner_EK746oGQz6E_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/audioset_realrec_barking_5F9Gd2JNcw8_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR2-L/audioset_realrec_barking_5F9Gd2JNcw8_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_car_0AVTgzegI4s.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/audioset_realrec_car_0AVTgzegI4s_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="MaskSR-L/audioset_realrec_car_0AVTgzegI4s_proc.wav"></audio></html></td>      
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_car_0AVTgzegI4s.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_car_0AVTgzegI4s.wav"></audio></html></td>
    </tr>
  </tbody>
</table>