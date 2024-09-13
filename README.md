# Joint Semantic Knowledge Distillation and Masked Acoustic Modeling for Full-band Speech Restoration with Improved Intelligibility

This is the demonstration page of the paper "Joint Semantic Knowledge Distillation and Masked Acoustic Modeling for Full-band Speech Restoration with Improved Intelligibility" with some selected samples generated with the proposed method.

## Abstract

Speech restoration aims at restoring full-band speech with
high quality and intelligibility, considering a diverse set of distortions.
MaskSR is a recently proposed generative model for this task. As other
models of its kind, MaskSR attains high quality but, as we show,
intelligibility can be substantially improved. We do so by boosting the
speech encoder component of MaskSR with predictions of semantic
representations of the target speech, using a pre-trained self-supervised teacher model. Then, a masked language model is conditioned on the learned semantic features to predict acoustic tokens that encode low level spectral details of the target speech. We show that, with the same MaskSR model capacity and inference time, the proposed model, MaskSR2, significantly reduces the word error rate, a typical metric for intelligibility. MaskSR2 also achieves competitive word error rate among other models, while providing superior quality. An ablation study shows the effectiveness of various semantic representations.
