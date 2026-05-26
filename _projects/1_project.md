---
layout: page
title: Model compression for multi-modal identity recognition
description: Inception-ResNet-v2 redesigned with 2D separable convolutions — 78% fewer parameters at 95.4% accuracy on images + audio.
importance: 1
category: research
img: assets/img/proj1.png
github: https://github.com/utsav-akhaury/Identity-Recognition
---

A multi-modal identity recognition system that classifies 49 individuals from facial images and audio. Built as a group project with my classmates *Frédéric Dux* and *Louis Suter*. The focus: aggressive model compression without giving up accuracy.

## Multi-modal pipeline

Two parallel encoders produce embeddings that are concatenated and passed to a small dense classifier:

- **Images** — `dlib` face detection → cropped face → Inception-ResNet-v2 (a 54M-parameter CNN that combines Inception modules with residual connections) → 49-D unit vector
- **Audio** — Mel-frequency cepstral analysis (MFCC, chroma, mel, contrast via *librosa*) → time-averaged coefficients → dense audio clusterer → 40-D vector

Both encoders are trained in two stages: first with **cross-entropy** loss for class separation (~80% on images), then fine-tuned with **triplet loss** (`D_positive − D_negative + 2`) to tighten the identity clusters (~94% on images, ~78% on audio).

## Compression via separable convolutions

Replaced standard convolutions in the image encoder with **2D depthwise-separable convolutions**, which factor a 5×5×3 kernel into a depthwise (5×5×1 per channel) plus a pointwise (1×1×3) step. On a 12×12×3 input with 256 output channels, this cuts the multiplications from **1,228,800 → 49,152 (~25× reduction)** with negligible accuracy loss.

<div class="row mt-3 justify-content-center">
  <div class="col-9">
    {% include figure.liquid loading="lazy" path="assets/img/proj1_sep_conv1.png" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="caption">
  Standard convolution with 256 5×5×3 kernels: ~1.23M multiplications.
</div>

<div class="row mt-3 justify-content-center">
  <div class="col-9">
    {% include figure.liquid loading="lazy" path="assets/img/proj1_sep_conv2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="caption">
  Depthwise + pointwise factorisation: ~49K multiplications, a 25× reduction with negligible accuracy loss.
</div>

## Backbone comparison

Custom metric: `accuracy − (parameters / 10⁷)`. Rewards accuracy while penalising parameter count.

| Backbone | Image Accuracy | Combined Accuracy | Params |
|---|---|---|---|
| ResNet50 + SeparableConv | 90.1% | 93.7% | 13.6M |
| Inception-ResNet-v2 *(baseline)* | 94.2% | 96.7% | 54.4M |
| Inception-ResNet-v2 + SeparableConv | 94.0% | 96.6% | 40.6M |
| **Truncated Inception-ResNet-v2 + SeparableConv** | **93.2%** | **95.4%** | **11.9M** |

## Result

The truncated Inception-ResNet-v2 with separable convolutions cuts model size from **54M → 11.9M parameters (~78% reduction)** while holding **95.4% test accuracy** on the combined image + audio task. The dense classifier on top of the joint embeddings adds only ~78K parameters, meaning new identities can be added by retraining a tiny head in seconds on CPU.

<i class="fa-brands fa-github"></i> **Code:** [github.com/utsav-akhaury/Identity-Recognition](https://github.com/utsav-akhaury/Identity-Recognition)
