---
layout: default
title: "CherainboowARTs"
permalink: /arts/
---

<style>
/* ── Morandi Neo-Brutalist Portfolio ── */
:root {
  --m-beige:  #E8E2D7;
  --m-rose:   #C9A9A6;
  --m-sage:   #8FAF8A;
  --m-blue:   #8BA7B8;
  --m-terra:  #C4846A;
  --m-lav:    #A89BB0;
  --m-warm:   #B5AFA8;
  --ink:      #2C2C2C;
}

.arts-page {
  font-family: "PT Sans", Helvetica, sans-serif;
  color: var(--ink);
  max-width: 860px;
  margin: 0 auto;
  padding: 0 0 4rem;
}

/* ── Hero ── */
.arts-hero {
  background: var(--m-beige);
  border: 3px solid var(--ink);
  box-shadow: 8px 8px 0 var(--ink);
  margin-bottom: 3rem;
  display: grid;
  grid-template-columns: 1fr 1.1fr;
  align-items: center;
  overflow: hidden;
  min-height: 280px;
}
.arts-hero-text {
  padding: 2.4rem 2rem 2.4rem 2.4rem;
  display: flex;
  flex-direction: column;
  gap: 0.7rem;
}
.arts-eyebrow {
  font-size: 0.6rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--m-warm);
}
.arts-hero h1 {
  font-family: "Abril Fatface", serif;
  font-size: clamp(2rem, 4vw, 3rem);
  line-height: 1.0;
  color: var(--ink);
  margin: 0;
  border: none;
}
.arts-hero h1 span { color: var(--m-rose); }
.arts-hero-sub {
  font-size: 0.78rem;
  color: var(--m-warm);
  line-height: 1.5;
  margin: 0;
}
.arts-hero-cta {
  display: inline-block;
  margin-top: 0.4rem;
  background: var(--ink);
  color: var(--m-beige) !important;
  padding: 0.55rem 1.4rem;
  font-size: 0.72rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  text-decoration: none;
  font-weight: 700;
  border: 2.5px solid var(--ink);
  box-shadow: 4px 4px 0 var(--m-rose);
  width: fit-content;
  transition: transform 0.15s, box-shadow 0.15s;
}
.arts-hero-cta:hover {
  transform: translate(-2px,-2px);
  box-shadow: 6px 6px 0 var(--m-rose);
}
.arts-hero-img {
  height: 280px;
  overflow: hidden;
  border-left: 3px solid var(--ink);
  background: #f5f0eb;
  display: flex;
  align-items: center;
  justify-content: center;
}
.arts-hero-img img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: left center;
  mix-blend-mode: multiply;
  background: #f5f0eb;
}

/* ── Section label ── */
.arts-section-label {
  display: block;
  font-size: 0.6rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--m-warm);
  margin-bottom: 1.2rem;
}

/* ── Works grid ── */
.arts-grid {
  columns: 2;
  column-gap: 1rem;
  margin-bottom: 3rem;
}
@media (min-width: 640px) { .arts-grid { columns: 3; } }

.arts-item {
  break-inside: avoid;
  margin-bottom: 1rem;
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--ink);
  overflow: hidden;
  background: var(--m-beige);
  display: block;
  text-decoration: none;
  transition: transform 0.15s, box-shadow 0.15s;
}
.arts-item:hover {
  transform: translate(-3px, -3px);
  box-shadow: 8px 8px 0 var(--ink);
}
.arts-item img {
  width: 100%;
  display: block;
  border-bottom: 2px solid var(--ink);
  transition: filter 0.3s;
  filter: saturate(0.75);
}
.arts-item:hover img { filter: saturate(1.1); }
.arts-item-label {
  padding: 0.5rem 0.75rem;
  font-size: 0.62rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--m-warm);
  font-weight: 700;
  background: var(--m-beige);
}

/* ── Quote ── */
.arts-quote {
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--m-rose);
  padding: 1.8rem 2rem;
  margin-bottom: 3rem;
  background: #fff;
  position: relative;
}
.arts-quote::before {
  content: '"';
  font-family: "Abril Fatface", serif;
  font-size: 6rem;
  color: var(--m-rose);
  opacity: 0.18;
  position: absolute;
  top: -1.5rem;
  left: 1rem;
  line-height: 1;
}
.arts-quote p {
  font-family: "Abril Fatface", serif;
  font-size: 1.05rem;
  line-height: 1.6;
  color: var(--ink);
  margin: 0 0 0.5rem;
  position: relative;
}
.arts-quote cite {
  font-size: 0.65rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--m-warm);
}

/* ── Color tag strip ── */
.arts-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 2rem;
}
.arts-tag {
  padding: 0.3rem 0.9rem;
  font-size: 0.62rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  font-weight: 700;
  border: 2px solid var(--ink);
  color: var(--ink);
}

/* ── Responsive ── */
@media (max-width: 600px) {
  .arts-hero { grid-template-columns: 1fr; }
  .arts-hero-img { border-left: none; border-top: 3px solid var(--ink); height: 200px; }
}
</style>

<div class="arts-page">

  <!-- Hero -->
  <div class="arts-hero">
    <div class="arts-hero-text">
      <span class="arts-eyebrow">— Visual Portfolio</span>
      <h1>Cherainboow<br><span>ARTs</span></h1>
      <p class="arts-hero-sub">Painting · Photography · Visual Storytelling</p>
      <a class="arts-hero-cta" href="https://www.instagram.com/cherainboow" target="_blank">↗ Instagram</a>
    </div>
    <div class="arts-hero-img">
      <img src="/public/image/hero-arts.png" alt="Cherainboow Arts" />
    </div>
  </div>

  <!-- Quote -->
  <div class="arts-quote">
    <p>To see a World in a Grain of Sand, and a Heaven in a Wild Flower.</p>
    <cite>— William Blake, Auguries of Innocence</cite>
  </div>

  <!-- Tags -->
  <span class="arts-section-label">— Works</span>
  <div class="arts-tags">
    <span class="arts-tag" style="background:var(--m-rose);border-color:var(--ink)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--m-sage);border-color:var(--ink)">Photography</span>
    <span class="arts-tag" style="background:var(--m-blue);border-color:var(--ink)">Illustration</span>
    <span class="arts-tag" style="background:var(--m-lav);border-color:var(--ink)">Mixed Media</span>
  </div>

  <!-- Grid -->
  <div class="arts-grid">

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/Oilp.JPG" alt="Oil Painting" />
      <div class="arts-item-label">Oil · 2024</div>
    </a>

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/Evergreen.JPG" alt="Evergreen" />
      <div class="arts-item-label">Evergreen</div>
    </a>

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/KAEO.PNG" alt="KAEO" />
      <div class="arts-item-label">KAEO</div>
    </a>

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/abg.JPG" alt="Abstract" />
      <div class="arts-item-label">Abstract</div>
    </a>

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/scottish-fantazy-cover.png" alt="Scottish Fantasy" />
      <div class="arts-item-label">Scottish Fantasy</div>
    </a>

    <a class="arts-item" href="https://www.instagram.com/cherainboow" target="_blank">
      <img src="/public/image/candy.png" alt="Candy" />
      <div class="arts-item-label">Candy</div>
    </a>

  </div>

  <p style="text-align:center;font-size:0.65rem;letter-spacing:0.18em;text-transform:uppercase;color:var(--m-warm);">
    More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:var(--m-rose);text-decoration:none;font-weight:700;">@cherainboow</a>
  </p>

</div>
