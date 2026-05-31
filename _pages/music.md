---
layout: page
permalink: /music/
title: Music
# description: "Pianist and electronic music producer — releases, collaborations, and a rotating shortlist of what I'm listening to."
nav: true
nav_order: 4
---

A chance encounter led me to the piano at the age of 8. What began as curiosity soon blossomed into an unbreakable bond with the keys. Every melody in the air became a puzzle for my fingers to decode. Over the years, my ear learnt to keep up, sharpening into near-perfect pitch. This bond has had me playing everywhere from Parisian bars to cultural events at the **United Nations**.

My background in Electronics Engineering and Astrophysics eventually found their way into my music. Signal processing shapes the way I produce, and a lifelong fascination with outer space shapes what I write.

Having lived in four countries across three continents, I'm endlessly drawn to the intricate details of music from around the world. After years of experimentation, improvisation, and a bit of procrastination, I'm finally proud to share my creative journey.

A few elements that can make me instantly like a song:
1. Odd time signatures and polyrhythms
2. Modal interchange — especially the minor plagal cadence (iv → I)
3. Modal colour notes like ♭2, ♯4, ♭6
4. Secondary dominants
5. Chromaticism

<style>
  .post p {
    text-align: left;
    overflow-wrap: break-word;
    hyphens: none;
  }
  .post h2 {
    border-top: 1px solid var(--global-divider-color);
    padding-top: 1.5rem;
  }
  a.music-header-link {
    color: var(--global-text-color);
    text-decoration: none;
    margin-left: 6px;
    font-size: 0.85em;
    vertical-align: middle;
    transition: color 120ms ease;
  }
  a.music-header-link:hover {
    color: var(--global-theme-color);
    text-decoration: none;
  }
  .yt-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 14px;
  }
  .yt-grid iframe {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: 0;
    border-radius: 12px;
  }
  .yt-shorts {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 14px;
    margin-top: 14px;
  }
  .yt-shorts iframe {
    width: 100%;
    aspect-ratio: 9 / 16;
    border: 0;
    border-radius: 12px;
  }
  @media (max-width: 576px) {
    .yt-grid { grid-template-columns: 1fr; }
    .yt-shorts { grid-template-columns: repeat(2, 1fr); }
  }
  .music-gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 2px 14px;
    margin-top: 2.5rem;
    margin-bottom: -1rem;
    align-items: flex-start;
  }
  .music-gallery > figure {
    flex: 0 1 275px;
    margin: 0;
    max-width: 100%;
  }
  .music-gallery > figure picture {
    display: block;
    width: 100%;
  }
  .music-gallery > figure img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 6px;
  }
  .music-gallery > figure figcaption {
    font-size: 0.875rem;
    line-height: 1.4;
    margin-top: 10px;
    /* color: color-mix(in srgb, var(--global-text-color) 25%, black); */
  }
  /* .music-gallery > figure figcaption::before {
    content: "* ";
  } */
</style>

## Highlights

<div class="music-gallery">
  {% include figure.liquid path="assets/img/music/UN.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Representing Indian music at UN Geneva, 2024" %}
  {% include figure.liquid path="assets/img/music/paris.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Taking requests from strangers at a Parisian bar, 2024" %}
  {% include figure.liquid path="assets/img/music/desk.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="My work desk during my PhD, 2024" %}
  {% include figure.liquid path="assets/img/music/obs.png" zoomable=true class="img-fluid rounded z-depth-1" caption="Jamming inside a nuclear bunker at the Geneva Observatory, 2024" %}
  {% include figure.liquid path="assets/img/music/drum.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Drumming with a view of Bangalore, 2026" %}
  {% include figure.liquid path="assets/img/music/chania.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Playing at the Chania Sailing Club, Greece, 2024" %}
  {% include figure.liquid path="assets/img/music/mall.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Forced by mom to play a public piano in a mall in Mumbai, 2018" %}
  {% include figure.liquid path="assets/img/music/car.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Spotted myself next to deadmau5 on someone's Spotify shortcuts, 2026" %}
  {% include figure.liquid path="assets/img/music/yuvaali.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Performing at a Swiss Diwali celebration in Lausanne, 2025" %}
  {% include figure.liquid path="assets/img/music/epfl.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Debut performance at EPFL, 2023" %}
  {% include figure.liquid path="assets/img/music/prod.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="My first bedroom production setup, 2018" %}
  {% include figure.liquid path="assets/img/music/coke.jpeg" zoomable=true class="img-fluid rounded z-depth-1" caption="Covering Coke Studio classics at BITS Pilani, 2017" %}  
  {% include figure.liquid path="assets/img/music/wrapped.png" zoomable=true class="img-fluid rounded z-depth-1" caption="My first Spotify wrapped as an artist, 2024" %}
  {% include figure.liquid path="assets/img/music/prod_2.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Upgrade made possible by a Swiss PhD salary, 2023" %}
  {% include figure.liquid path="assets/img/music/dj.jpg" zoomable=true class="img-fluid rounded z-depth-1" caption="Behind the decks in Crete, Greece, 2024" %}
</div>


## Releases

If you want to hear what I've actually finished, the originals are on Spotify, YouTube, and Apple Music. The covers, jam sessions, and mashups I can't help posting go up on Instagram.

<div class="d-flex flex-wrap gap-2 mb-3">
  <a class="btn btn-sm btn-outline-primary" href="https://open.spotify.com/artist/6Z4HMMabdi0YCphd4HaMus" target="_blank" rel="noopener"><i class="fa-brands fa-spotify"></i> Spotify</a>
  <a class="btn btn-sm btn-outline-danger" href="https://youtube.com/@UtsavAkhaury" target="_blank" rel="noopener"><i class="fa-brands fa-youtube"></i> YouTube</a>
  <a class="btn btn-sm" style="color: #FA243C; border: 1px solid #FA243C;" href="https://music.apple.com/us/artist/utsav-akhaury/1644561545" target="_blank" rel="noopener"><i class="fa-brands fa-apple"></i> Apple Music</a>
  <a class="btn btn-sm" style="color: #E1306C; border: 1px solid #E1306C;" href="https://www.instagram.com/utsav_akhaury/" target="_blank" rel="noopener"><i class="fa-brands fa-instagram"></i> Instagram</a>
</div>

## Spotify <a class="music-header-link" href="https://open.spotify.com/artist/6Z4HMMabdi0YCphd4HaMus" target="_blank" rel="noopener" title="Open on Spotify"><i class="fa-brands fa-spotify"></i></a>

<iframe
  style="border-radius:12px"
  src="https://open.spotify.com/embed/artist/6Z4HMMabdi0YCphd4HaMus?utm_source=generator"
  width="100%"
  height="352"
  frameborder="0"
  allowfullscreen=""
  allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
  loading="lazy">
</iframe>

## YouTube <a class="music-header-link" href="https://youtube.com/@UtsavAkhaury" target="_blank" rel="noopener" title="Open on YouTube"><i class="fa-brands fa-youtube"></i></a>


<div class="yt-grid">
  <iframe
    src="https://www.youtube.com/embed/r5V7XWV1HNs"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
  <iframe
    src="https://www.youtube.com/embed/svzmKVacbZ0"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
</div>


<div class="yt-shorts">
  <iframe
    src="https://www.youtube.com/embed/-EEd9PGgCYU"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
  <iframe
    src="https://www.youtube.com/embed/jd7UpgmspCM"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
  <iframe
    src="https://www.youtube.com/embed/Fe-ZqsOJPW8"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
  <iframe
    src="https://www.youtube.com/embed/CgZ7N7b8R3w"
    allowfullscreen
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    loading="lazy">
  </iframe>
</div>







