---
layout: default
title: "CherainboowARTs"
permalink: /arts/
---

<link href="https://fonts.googleapis.com/css2?family=Righteous&family=PT+Sans:wght@400;700&display=swap" rel="stylesheet">

<style>
@font-face {
  font-family: 'Pagkaki';
  src: url('/public/fonts/PAGKAKI-Regular.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}

:root {
  --m-beige:  #E8E2D7;
  --m-rose:   #C9A9A6;
  --m-sage:   #8FAF8A;
  --m-blue:   #8BA7B8;
  --m-terra:  #C4846A;
  --m-lav:    #A89BB0;
  --m-warm:   #B5AFA8;
  --ink:      #2C2C2C;
  /* Macaroon palette */
  --mac-rose:   #F2B5C0;
  --mac-mint:   #B5E8D5;
  --mac-lemon:  #F7E8A0;
  --mac-lav:    #C9B8E8;
  --mac-sky:    #A8D8EA;
  --mac-peach:  #F5C9A8;
}

.arts-page {
  font-family: "PT Sans", sans-serif;
  color: var(--ink);
  max-width: 900px;
  margin: 0 auto;
  padding: 0 0 4rem;
}

/* ── Hero ── */
.arts-hero {
  position: relative;
  background: #0d0d0d;
  border: 3px solid #1a1a1a;
  border-bottom: none;
  box-shadow: none;
  margin-bottom: 0;
  overflow: hidden;
  min-height: 360px;
}

/* Full illustration as background */
.arts-hero-bg {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
}

/* Title bar below hero */
.arts-poster-bar {
  background: #0d0d0d;
  border: 3px solid #1a1a1a;
  border-top: none;
  box-shadow: 8px 8px 0 #1a1a1a;
  padding: 1.2rem 1.8rem 1.4rem;
  margin-bottom: 2.5rem;
}

.arts-poster {
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
}

.hw {
  display: inline-block;
  font-family: 'Pagkaki', 'Righteous', cursive;
  line-height: 1.1;
  padding: 0.08em 0.24em;
  position: relative;
}
.hw-cherainboow {
  font-size: clamp(1.8rem, 4vw, 3rem);
  background: var(--mac-rose);
  color: #2C2C2C;
  transform: rotate(-1.5deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.45);
}
.hw-arts {
  font-size: clamp(2.2rem, 5vw, 3.8rem);
  background: var(--mac-mint);
  color: #2C2C2C;
  transform: rotate(1deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.45);
  margin-left: 0.15em;
}
.hw-sub {
  font-family: 'Righteous', sans-serif;
  font-size: clamp(0.68rem, 1.4vw, 0.9rem);
  color: rgba(255,255,255,0.7);
  letter-spacing: 0.06em;
  display: block;
  padding: 0;
  margin-top: 0.3rem;
}

.arts-poster-ig {
  margin-top: 0.7rem;
  display: inline-block;
  background: transparent;
  color: var(--mac-lemon) !important;
  padding: 0.35rem 1rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-decoration: none;
  border: 2px solid var(--mac-lemon);
  box-shadow: 3px 3px 0 var(--mac-lemon);
  width: fit-content;
  transition: transform 0.15s, box-shadow 0.15s, background 0.15s;
}
.arts-poster-ig:hover {
  background: var(--mac-lemon);
  color: #2C2C2C !important;
  transform: translate(-2px,-2px);
  box-shadow: 5px 5px 0 var(--mac-lemon);
}

/* ── Quote ── */
.arts-quote {
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--mac-rose);
  padding: 1.5rem 1.8rem;
  margin-bottom: 2.5rem;
  background: #0d0d0d;
}
.arts-quote p {
  font-family: 'Pagkaki', 'Righteous', cursive;
  font-size: clamp(1rem, 2vw, 1.2rem);
  line-height: 1.7;
  color: #fff;
  margin: 0 0 0.4rem;
}
.arts-quote p .qart { color: var(--mac-rose); }
.arts-quote p .qsci { color: var(--mac-sky); }
.arts-quote cite {
  font-size: 0.6rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.4);
  font-family: "PT Sans", sans-serif;
}

/* ── Tags ── */
.arts-section-label {
  display: block;
  font-size: 0.6rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--m-warm);
  margin-bottom: 1.2rem;
}
.arts-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 2rem;
}
.arts-tag {
  padding: 0.28rem 0.85rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.7rem;
  border: 2px solid var(--ink);
  color: var(--ink);
  letter-spacing: 0.04em;
}

/* ── Grid ── */
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
  transform: translate(-3px,-3px);
  box-shadow: 8px 8px 0 var(--ink);
}
.arts-item img {
  width: 100%;
  display: block;
  border-bottom: 2px solid var(--ink);
  filter: saturate(0.72);
  transition: filter 0.3s;
}
.arts-item:hover img { filter: saturate(1.15); }
.arts-item-label {
  padding: 0.45rem 0.75rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.68rem;
  color: var(--m-warm);
  letter-spacing: 0.06em;
}

@media (max-width: 540px) {
  .arts-hero { min-height: 220px; }
  .arts-poster-bar { padding: 1rem 1rem 1.2rem; }
}
</style>

<div class="arts-page">

  <!-- Hero: illustration only -->
  <div class="arts-hero">
    <img class="arts-hero-bg" src="/public/image/hero-arts.png" alt="Cherainboow Arts" />
  </div>

  <!-- Title bar below the image -->
  <div class="arts-poster-bar">
    <div class="arts-poster">
      <div>
        <span class="hw hw-cherainboow">Cherainboow</span>
        <span class="hw hw-arts">ARTs</span>
      </div>
      <span class="hw-sub">Portrait · Landscape · Watercolour · Procreate · Illustration</span>
      <a class="arts-poster-ig" href="https://www.instagram.com/cherainboow" target="_blank">↗ @cherainboow</a>
    </div>
  </div>

  <!-- Quote -->
  <div class="arts-quote">
    <p>Wish to use <span class="qart">"Art"</span> to see the World<br>and <span class="qsci">"Science"</span> to color the Nature.</p>
    <cite>— Cherub</cite>
  </div>

  <!-- Media tags -->
  <span class="arts-section-label">— Mediums</span>
  <div class="arts-tags">
    <span class="arts-tag" style="background:var(--mac-rose);border-color:var(--ink)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--mac-lemon);border-color:var(--ink)">Watercolour</span>
    <span class="arts-tag" style="background:var(--mac-mint);border-color:var(--ink)">Acrylic</span>
    <span class="arts-tag" style="background:var(--mac-sky);border-color:var(--ink)">Procreate</span>
    <span class="arts-tag" style="background:var(--mac-lav);border-color:var(--ink)">Mixed Media</span>
    <span class="arts-tag" style="background:var(--m-warm);border-color:var(--ink)">Charcoal</span>
    <span class="arts-tag" style="background:var(--mac-peach);border-color:var(--ink)">Oil Pastel</span>
    <span class="arts-tag" style="background:var(--m-beige);border-color:var(--ink)">Illustration</span>
  </div>

  <!-- Works -->
  <span class="arts-section-label">— Works</span>
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

  <p style="text-align:center;font-family:'Righteous',sans-serif;font-size:0.72rem;letter-spacing:0.1em;color:var(--m-warm);">
    More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:var(--mac-rose);text-decoration:none;">@cherainboow</a>
  </p>

</div>
