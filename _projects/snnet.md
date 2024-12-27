---
layout: page
title: My implementation of SN-Net
description: audio sample processed with SN-Net implemented by me
img: assets/img/projects/snnet/1.png
importance: 1
category: work
pretty_table: true
---

## Interactive Speech and Noise Modeling for Speech Enhancement

**Authors**: Chengyu Zheng, Xiulian Peng, Yuan Zhang, Sriram Srinivasan, Yan Lu

---

### Links
The paper is available at both [English Version](https://arxiv.org/pdf/2012.09408) and [中文翻译版](https://blog.csdn.net/wjrenxinlei/article/details/122670688)。

---

### Demo
I implemented SN-Net and processed several audio samples here.

<table style="text-align: center;">
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