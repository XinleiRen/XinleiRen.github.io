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

**Authors**: Chengyu Zheng^1^, Xiulian Peng^2^, Yuan Zhang^1^, Sriram Srinivasan^3^, Yan Lu^2^
**Affiliation**: ^1^Communication University of China, ^2^Microsoft Research Asia, ^3^Microsoft Corporation

---

### Abstract
Speech enhancement is challenging because of the diversity of background noise types. Most of the existing methods are focused on modelling the speech rather than the noise. In this paper, we propose a novel idea to model speech and noise simultaneously in a two-branch convolutional neural network, namely SN-Net. In SN-Net, the two branches predict speech and noise, respectively. Instead of information fusion only at the final output layer, interaction modules are introduced at several intermediate feature domains between the two branches to benefit each other. Such an interaction can leverage features learned from one branch to counteract the undesired part and restore the missing component of the other and thus enhance their discrimination capabilities. We also design a feature extraction module, namely residual-convolution-and-attention (RA), to capture the correlations along temporal and frequency dimensions for both the speech and the noises. Evaluations on public datasets show that the interaction module plays a key role in simultaneous modeling and the SN-Net outperforms the state-of-the-art by a large margin on various evaluation metrics. The proposed SN-Net also shows superior performance for speaker separation.

---

### System Architecture

{% include figure.liquid loading="eager" path="assets/img/projects/1.png" title="SN-Net Architecture" class="img-fluid rounded z-depth-1" %}

---

### Demo

<table>
    <tr>
        <td> </td>
        <th>noisy</th>
        <th>denoised</th>
    </tr>
    <tr>
        <td rowspan="2">sample 1</td>
        <td><img src="assets/img/projects/snnet/samp1_noisy.jpeg" width="305" height="250" /></td>
        <td><img src="assets/img/projects/snnet/samp1_denoised.jpeg" width="305" height="250" /></td>
    </tr>
    <tr>
        <td><audio controls src="assets/audio/projects/snnet/samp1_noisy.wav"></audio></td>
        <td><audio controls src="assets/audio/projects/snnet/samp1_denoised.wav"></audio></td>
    </tr>
</table>
