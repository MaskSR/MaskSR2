
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
      <td>
        <html>
          <audio controls>
            <source src="dag_audio/air_conditioner_0.wav">
          </audio>
        </html>
      </td>
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
      <td><html><audio controls preload><source src="GSR/Unprocessed/8_simulated.wav"></audio></html></td>
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

#### From 1kHz to 44.1kHz

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
      <td><html><audio controls><source src="SR/Unprocessed/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p360_354_mic1_1000_cheby1.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p363_283_mic1_1000_cheby1.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

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
      <td><html><audio controls><source src="SR/Unprocessed/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p360_275_mic1_2000_cheby1.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p363_037_mic1_2000_cheby1.wav"></audio></html></td>
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
      <td><html><audio controls><source src="SR/Unprocessed/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p361_084_mic1_4000_cheby1.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p364_249_mic1_4000_cheby1.wav"></audio></html></td>
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
      <td><html><audio controls><source src="SR/Unprocessed/p376_030_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/p376_030_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/p376_030_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/p376_030_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/p376_030_mic1_8000_cheby1.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="SR/Unprocessed/s5_356_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/Target/s5_356_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/MaskSR-M/s5_356_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/VoiceFixer/s5_356_mic1_8000_cheby1.wav"></audio></html></td>
      <td><html><audio controls><source src="SR/NSNet2/s5_356_mic1_8000_cheby1.wav"></audio></html></td>
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
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp177_0kuIP7fLNpM_snr6_tl-26_fileid_90.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/MaskSR/clnsp177_0kuIP7fLNpM_snr6_tl-26_fileid_90.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp177_0kuIP7fLNpM_snr6_tl-26_fileid_90.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp177_0kuIP7fLNpM_snr6_tl-26_fileid_90.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/MaskSR/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp25_babble_188218_21_snr5_tl-25_fileid_147.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/MaskSR/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp62_birds_413745_6_snr14_tl-33_fileid_81.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_no_reverb/noisy/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/MaskSR/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/FRCRN/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_no_reverb/DEMUCS/clnsp71_babble_188218_26_snr4_tl-20_fileid_275.wav"></audio></html></td>
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
      <td><html><audio controls><source src="DNS2020_with_reverb/noisy/clnsp1_train_69005_1_snr15_tl-21_fileid_158.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/MaskSR/clnsp1_train_69005_1_snr15_tl-21_fileid_158.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/FRCRN/clnsp1_train_69005_1_snr15_tl-21_fileid_158.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/DEMUCS/clnsp1_train_69005_1_snr15_tl-21_fileid_158.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_with_reverb/noisy/clnsp27_GvaTLOWuCK8_snr10_tl-22_fileid_296.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/MaskSR/clnsp27_GvaTLOWuCK8_snr10_tl-22_fileid_296.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/FRCRN/clnsp27_GvaTLOWuCK8_snr10_tl-22_fileid_296.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/DEMUCS/clnsp27_GvaTLOWuCK8_snr10_tl-22_fileid_296.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_with_reverb/noisy/clnsp30_birds_121947_2_snr6_tl-27_fileid_116.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/MaskSR/clnsp30_birds_121947_2_snr6_tl-27_fileid_116.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/FRCRN/clnsp30_birds_121947_2_snr6_tl-27_fileid_116.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/DEMUCS/clnsp30_birds_121947_2_snr6_tl-27_fileid_116.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_with_reverb/noisy/clnsp51_baby_416672_0_snr11_tl-22_fileid_167.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/MaskSR/clnsp51_baby_416672_0_snr11_tl-22_fileid_167.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/FRCRN/clnsp51_baby_416672_0_snr11_tl-22_fileid_167.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_with_reverb/DEMUCS/clnsp51_baby_416672_0_snr11_tl-22_fileid_167.wav"></audio></html></td>
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
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/MaskSR/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_airconditioner_8v4sEeK2Owc.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/MaskSR/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_airconditioner_EK746oGQz6E.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/MaskSR/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_barking_5F9Gd2JNcw8.wav"></audio></html></td>
    </tr>
    <tr>
      <td><html><audio controls><source src="DNS2020_real_recordings/noisy/audioset_realrec_barking_9uNc2tH5aV4.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/MaskSR/audioset_realrec_barking_9uNc2tH5aV4.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/FRCRN/audioset_realrec_barking_9uNc2tH5aV4.wav"></audio></html></td>
      <td><html><audio controls><source src="DNS2020_real_recordings/DEMUCS/audioset_realrec_barking_9uNc2tH5aV4.wav"></audio></html></td>
    </tr>
  </tbody>
</table>

