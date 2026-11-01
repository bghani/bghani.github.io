---
layout: page
title: code & projects
permalink: /code/
description: Open tools for working with animal sound, and things built with them.
nav: true
nav_order: 2
---

<style>
  .cp-intro { color: var(--global-text-color-light); margin-bottom: 2.5rem; }
  .cp-label {
    font-size: 0.75rem; letter-spacing: 0.15em; text-transform: uppercase;
    color: var(--global-text-color-light); margin: 3rem 0 0.5rem;
  }
  .cp-item {
    display: grid; grid-template-columns: 11rem 1fr; gap: 0.25rem 2rem;
    padding: 1.5rem 0; border-top: 1px solid var(--global-divider-color);
  }
  .cp-item:last-of-type { border-bottom: 1px solid var(--global-divider-color); }
  .cp-name {
    font-family: var(--font-family-monospace); font-weight: 600;
    font-size: 1rem; padding-top: 0.15rem;
  }
  .cp-name a { color: var(--global-text-color); }
  .cp-name a:hover { color: var(--global-theme-color); text-decoration: none; }
  .cp-body p { margin: 0 0 0.6rem; }
  .cp-cmd {
    display: inline-block; font-family: var(--font-family-monospace);
    font-size: 0.8rem; padding: 0.2rem 0.6rem; border-radius: 4px;
    background: var(--global-code-bg-color);
  }
  .cp-cmd::before { content: "$ "; color: var(--global-text-color-light); }
  .cp-meta {
    font-size: 0.8rem; color: var(--global-text-color-light); margin-top: 0.6rem;
  }
  .cp-meta a { color: var(--global-text-color-light); border-bottom: 1px solid currentColor; }
  .cp-meta a:hover { color: var(--global-theme-color); text-decoration: none; }
  .cp-feature img {
    width: 100%; border-radius: 6px; margin: 0.5rem 0 1rem;
    border: 1px solid var(--global-divider-color);
  }
  .cp-placeholder {
    display: flex; align-items: center; justify-content: center;
    aspect-ratio: 16 / 9; border-radius: 6px; margin: 0.5rem 0 1rem;
    border: 1px dashed var(--global-divider-color);
    background: var(--global-code-bg-color); color: var(--global-text-color-light);
  }
  .cp-feature h3 { font-weight: 400; margin: 0 0 0.5rem; }
  @media (max-width: 640px) {
    .cp-item { grid-template-columns: 1fr; }
  }
</style>

<p class="cp-intro">Most of these began as something I needed for my own research and turned out to be useful to others. Each one does one job, and all of them are open.</p>

<div class="cp-label">Software</div>

<div class="cp-item">
  <div class="cp-name"><a href="https://github.com/bghani/xcapi">xcapi</a></div>
  <div class="cp-body">
    <p>Download animal sound recordings and metadata from Xeno-canto, from the command line or in Python. Filter by species, place, date, quality, sample rate and more. Re-running a query fetches only what's new, so datasets can grow without duplicates.</p>
    <span class="cp-cmd">pip install xenocanto-api</span>
    <div class="cp-meta">Python · CLI · MIT · <a href="https://github.com/bghani/xcapi">GitHub</a></div>
  </div>
</div>

<div class="cp-item">
  <div class="cp-name"><a href="https://github.com/bghani/perchv2-pytorch">perchv2-pytorch</a></div>
  <div class="cp-body">
    <p>A trainable PyTorch port of Google's Perch v2 bioacoustic model. Extract embeddings, train a linear probe, or fine-tune the full backbone. The port is converted node by node from the released model and verified to match its outputs.</p>
    <span class="cp-cmd">git clone https://github.com/bghani/perchv2-pytorch</span>
    <div class="cp-meta">Python · PyTorch · Apache 2.0 · Unofficial port · <a href="https://github.com/bghani/perchv2-pytorch">GitHub</a></div>
  </div>
</div>

<div class="cp-item">
  <div class="cp-name"><a href="https://github.com/bghani/zenodo-uploader">zenodo-uploader</a></div>
  <div class="cp-body">
    <p>Upload large datasets to Zenodo without the browser timing out. Compresses directories automatically, retries failed transfers and verifies checksums, from the command line or in Python.</p>
    <span class="cp-cmd">pip install git+https://github.com/bghani/zenodo-uploader</span>
    <div class="cp-meta">Python · CLI · Builds on code by Pranav Durai · <a href="https://github.com/bghani/zenodo-uploader">GitHub</a></div>
  </div>
</div>

<div class="cp-label">Projects</div>

<div class="cp-feature">
  {%- assign kaetij_img = site.static_files | where: "path", "/assets/img/kaetij.png" | first %}
  {%- if kaetij_img %}
  <a href="https://kaetij.com"><img src="{{ '/assets/img/kaetij.png' | relative_url }}" alt="The Bioacoustic Map of Kashmir, showing recordings on a map alongside an embedding view"></a>
  {%- else %}
  <a href="https://kaetij.com" class="cp-placeholder">Screenshot coming soon</a>
  {%- endif %}
  <h3><a href="https://kaetij.com">Kaetij</a> · Bioacoustic Map of Kashmir</h3>
  <p>Kashmir's animal sounds, explored two ways: on a map of where each one was recorded, and in an embedding space where similar sounds sit close together. Click any point to hear it. Every recording comes from Xeno-canto, and the site invites people to add more.</p>
  <div class="cp-meta">Next.js · Leaflet · Three.js · <a href="https://kaetij.com">kaetij.com</a></div>
</div>
