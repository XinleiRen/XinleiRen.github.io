---
layout: page
title: SN-Net
description: audio sample of SN-Net
img: assets/img/projects/snnet/1.png
importance: 1
category: work
pretty_table: true
---

## Interactive Speech and Noise Modeling for Speech Enhancement

**Authors**: Chengyu Zheng, Xiulian Peng, Yuan Zhang, Sriram Srinivasan, Yan Lu

---

### Abstract
Speech enhancement is challenging because of the diversity of background noise types. Most of the existing methods are focused on modelling the speech rather than the noise. In this paper, we propose a novel idea to model speech and noise simultaneously in a two-branch convolutional neural network, namely SN-Net. In SN-Net, the two branches predict speech and noise, respectively. Instead of information fusion only at the final output layer, interaction modules are introduced at several intermediate feature domains between the two branches to benefit each other. Such an interaction can leverage features learned from one branch to counteract the undesired part and restore the missing component of the other and thus enhance their discrimination capabilities. We also design a feature extraction module, namely residual-convolution-and-attention (RA), to capture the correlations along temporal and frequency dimensions for both the speech and the noises. Evaluations on public datasets show that the interaction module plays a key role in simultaneous modeling and the SN-Net outperforms the state-of-the-art by a large margin on various evaluation metrics. The proposed SN-Net also shows superior performance for speaker separation.

---

### System Architecture

{% include figure.liquid loading="eager" path="assets/img/projects/snnet/1.png" title="SN-Net Architecture" class="img-fluid rounded z-depth-1" %}

---

### Demo

<table>
    <tr>
        <th> </th>
        <th>noisy</th>
        <th>denoised</th>
    </tr>
    <tr>
        <th rowspan="2">sample 1</th>
        <td>{% include audio.liquid path="assets/audio/projects/snnet/samp1_noisy.wav" controls=true %}</td>
        <td>{% include audio.liquid path="assets/audio/projects/snnet/samp1_denoised.wav" controls=true %}</td>
    </tr>
</table>
