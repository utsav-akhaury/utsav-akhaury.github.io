---
layout: about
title: About
permalink: /
description: "Personal site of Utsav Akhaury — AI Software Engineer building Agentic Vision."
# subtitle: "AI Software Engineer @ <a href='https://spot.ai'>Spot AI</a> — building <i>Agentic Vision</i>: AI that sees, reasons, and acts on real-time video."

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true
  # more_info: >
  #   <p>San Francisco, CA</p>
  #   <p>utsav.akhaury.2015 [at] gmail.com</p>

selected_papers: false
social: true

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

I'm an engineer with a long-standing passion for AI/ML and computer vision — one I turned into a PhD.

I now apply that foundation as an AI Software Engineer at [Spot AI](https://spot.ai), working on _Agentic Vision_ — AI that sees, reasons, and acts on real-time video.

I hold a PhD in Physics from [École Polytechnique Fédérale de Lausanne (EPFL)](https://infoscience.epfl.ch/entities/publication/bc2e9888-d73a-47f6-bdd6-630621730fec). My thesis focused on deep learning–based image enhancement, working with data from flagship NASA and European Space Agency (ESA) missions like _Hubble_, _James Webb_, and _Euclid_.

Across 5+ years, I've built, trained, and shipped ML systems from prototype to production, with deep experience in HPC environments (multi-node GPU training, distributed data pipelines). In 2021, I was a [Google Summer of Code](https://summerofcode.withgoogle.com/archive/2021/projects/5922912141312000) contributor, building ML surrogates for physics-based simulation.

## What I work on

<div class="work-row">
  <span class="skill-pill skill-pill--lead">Foundation encoders</span>
  <span class="work-desc">Vision and image–text embeddings for retrieval and transfer learning (MobileCLIP, SigLIP, DINOv2/v3)</span>
</div>
<div class="work-row">
  <span class="skill-pill skill-pill--lead">Multi-modality</span>
  <span class="work-desc">VLMs for natural-language video search and reasoning</span>
</div>
<div class="work-row">
  <span class="skill-pill skill-pill--lead">Perception</span>
  <span class="work-desc">Detection, tracking, and segmentation for real-time video (YOLO, ByteTrack, SAM 2)</span>
</div>
<div class="work-row">
  <span class="skill-pill skill-pill--lead">Restoration</span>
  <span class="work-desc">Denoising, deconvolution, and super-resolution for astronomical imaging (U-Net, ViT, Swin Transformer)</span>
</div>


## Tech I work with

<style>
  .post p {
    text-align: left;
  }
  .skill-pill {
    display: inline-block;
    padding: 3px 12px;
    margin: 0 4px 6px 0;
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.85em;
    line-height: 1.5;
    color: var(--global-text-color);
    background: var(--global-bg-color);
    transition: all 120ms ease;
  }
  .skill-pill:hover {
    background: var(--global-theme-color);
    border-color: var(--global-theme-color);
    color: var(--global-bg-color);
  }
  .skill-pill--lead {
    font-weight: 600;
  }
  .skill-row { margin-bottom: 12px; }
  .skill-row > strong { margin-right: 10px; }

  .work-row {
    display: flex;
    align-items: baseline;
    gap: 10px;
    margin-bottom: 15px;
  }
  .work-row > .skill-pill { margin: 0; flex: 0 0 auto; }
  .work-desc { flex: 1; line-height: 1.6; }

  .profile.float-right { margin-left: 4rem; }
  .profile.float-left  { margin-right: 4rem; }

  .post > article > .social { display: none; }
  .profile .social {
    display: block;
    text-align: center;
    margin-top: 14px;
  }
  .profile .contact-icons {
    font-size: 1.55rem;
    line-height: 1.5;
  }
  .profile .contact-icons a { margin: 0 3px; }
  .profile .contact-note { display: none; }

  @media (max-width: 575.98px) {
    .profile { margin-bottom: 1.75rem; }
  }
</style>

<script>
  (function () {
    function move() {
      var profile = document.querySelector('.post > article > .profile');
      var social = document.querySelector('.post > article > .social');
      if (profile && social) profile.appendChild(social);
    }
    if (document.readyState === 'loading') {
      document.addEventListener('DOMContentLoaded', move);
    } else {
      move();
    }
  })();
</script>

<div class="skill-row">
  <strong>Languages</strong>
  <span class="skill-pill">Python</span>
  <span class="skill-pill">C++</span>
  <span class="skill-pill">Julia</span>
  <span class="skill-pill">MATLAB</span>
  <span class="skill-pill">Rust</span>
</div>

<div class="skill-row">
  <strong>ML / Deep Learning</strong>
  <span class="skill-pill">PyTorch</span>
  <span class="skill-pill">CUDA</span>
  <span class="skill-pill">Hugging Face</span>
  <span class="skill-pill">TensorFlow</span>
  <span class="skill-pill">scikit-learn</span>
</div>

<div class="skill-row">
  <strong>Computer Vision</strong>
  <span class="skill-pill">OpenCV</span>
  <span class="skill-pill">ONNX</span>
  <span class="skill-pill">TensorRT</span>
  <span class="skill-pill">FFmpeg</span>
</div>

<div class="skill-row">
  <strong>MLOps &amp; Tooling</strong>
  <span class="skill-pill">Slurm</span>
  <span class="skill-pill">Docker</span>
  <span class="skill-pill">Kubernetes</span>
  <span class="skill-pill">Google Cloud</span>
  <span class="skill-pill">GitHub Actions</span>
</div>

## Outside work

My journey has taken me across India, Mauritius, France, and Switzerland, making me quietly obsessed with linguistics.

Along the way, I've developed a creative side as a pianist and electronic music producer. I've been playing piano since the age of 8 and have performed live at venues ranging from Parisian bars to cultural events at the **United Nations, Geneva**. Check out my compositions and covers on the [music](/music/) page.

<!-- The best way to reach me is by email. -->
