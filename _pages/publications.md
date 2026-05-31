---
layout: page
permalink: /publications/
title: Research
description: "Peer-reviewed publications by Utsav Akhaury — journal articles, conference proceedings, posters, and talks in deep learning and image restoration."
nav: true
nav_order: 1
---

Peer-reviewed journal articles, conference proceedings, posters, and talks — in reverse chronological order.

<style>
  .post h2 {
    border-top: 1px solid var(--global-divider-color);
    padding-top: 1.5rem;
  }
</style>

## PhD thesis

<div class="publications">
{% bibliography -q @phdthesis --group_by none %}
</div>

## Peer-reviewed journal articles

<div class="publications">
{% bibliography -q @article --group_by none %}
</div>

## Conference proceedings and posters

<div class="publications">
{% bibliography -q @inproceedings --group_by none %}
</div>

## Contributed talks

<div class="publications">
{% bibliography -q @misc --group_by none %}
</div>
