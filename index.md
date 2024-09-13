
# Joint Semantic Knowledge Distillation and Masked Acoustic Modeling for Full-band Speech Restoration with Improved Intelligibility

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
      <th>Improved works</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p360_018_272.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/1_clean.wav"></audio></html></td>
      <th>Aristotle thought that the rainbow was caused by reflection of the sun's rays by the rain.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p360_018_272_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p360_018_272_proc.wav"></audio></html></td>
      <th>by</th> 
    </tr>
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/2_simulated.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/2_simulated.wav"></audio></html></td>
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
      <td><html><audio controls><source src="For_intelligibility_table/target/10_simulated.wav"></audio></html></td>
      <th>I have so much respect for him. His friend</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/10_simulated_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/10_simulated_proc.wav"></audio></html></td>
      <th>for</th> 
    </tr>  
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/P361_174_66.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/P361_174_66.wav"></audio></html></td>
      <th>The quality of life is difficult for them.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/P361_174_66_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/P361_174_66_proc.wav"></audio></html></td>
      <th>life, difficult</th> 
    </tr>    
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/P362_158_555.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/P362_158_555.wav"></audio></html></td>
      <th>However, the story has a happy ending.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/P362_158_555_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/P362_158_555_proc.wav"></audio></html></td>
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
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/P363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/P363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <th>And the other winners are.</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/P363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/P363_283_mic1_1000_cheby1_proc.wav"></audio></html></td>
      <th>other</th> 
    </tr>     
    <tr>
      <td><html><audio controls><source src="For_intelligibility_table/unprocessed/p374_120_364.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/target/p374_120_364.wav"></audio></html></td>
      <th>That's not going to happen again</th>
      <td><html><audio controls><source src="For_intelligibility_table/masksr_L/p374_120_364_proc.wav"></audio></html></td>
      <td><html><audio controls><source src="For_intelligibility_table/masksr2_L/p374_120_364_proc.wav"></audio></html></td>
      <th>not</th> 
    </tr>                                   
  </tbody>
</table>