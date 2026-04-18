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
  --m-warm:   #B5AFA8;
  --ink:      #2C2C2C;
  --mac-rose:   #F2B5C0;
  --mac-mint:   #B5E8D5;
  --mac-lemon:  #F7E8A0;
  --mac-lav:    #C9B8E8;
  --mac-sky:    #A8D8EA;
  --mac-peach:  #F5C9A8;
}

/* ── Page wrapper ── */
.arts-page {
  font-family: "PT Sans", sans-serif;
  color: #fff;
  background: #0d0d0d;
  max-width: 900px;
  margin: 0 auto;
  padding: 0 0 4rem;
  border: 3px solid #2a1050;
  box-shadow: 10px 10px 0 #1a0838;
}

/* ── Hero ── */
.arts-hero {
  position: relative;
  background: #3D1F6E;
  overflow: hidden;
}
.arts-hero-bg {
  display: block;
  width: 100%;
  height: auto;
  object-fit: cover;
}

/* ── Instagram link overlaid bottom-center ── */
.arts-poster-ig {
  position: absolute;
  bottom: 1rem;
  left: 1.5rem;
  display: inline-block;
  background: transparent;
  color: #ffffff !important;
  padding: 0.3rem 1rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-decoration: none;
  white-space: nowrap;
  transition: background 0.15s, border-color 0.15s;
}
.arts-poster-ig:hover {
  color: #E8642A !important;
}

/* ── Quote ── */
.arts-quote {
  border-top: 1px solid #2a1050;
  border-bottom: 1px solid #2a1050;
  padding: 1.5rem 2rem;
  margin-bottom: 0;
  background: #1a0838;
}
.arts-quote p {
  font-family: 'Pagkaki', cursive;
  font-size: clamp(1rem, 2vw, 1.2rem);
  line-height: 1.7;
  color: #fff;
  margin: 0 0 0.4rem;
}
.arts-quote p .qart { color: var(--mac-rose); }
.arts-quote p .qsci { color: var(--mac-sky); }
.arts-quote cite {
  font-size: 0.58rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.35);
  font-family: "PT Sans", sans-serif;
}

/* ── Tags ── */
.arts-section-label {
  display: block;
  font-size: 0.58rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.35);
  margin-bottom: 1rem;
  padding: 1.4rem 2rem 0;
}
.arts-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 0;
  padding: 0 2rem 1.6rem;
}
.arts-tag {
  padding: 0.25rem 0.8rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.68rem;
  border: 2px solid rgba(255,255,255,0.15);
  color: #1a1a1a;
  letter-spacing: 0.04em;
}

/* ── Works label ── */
.arts-works-label {
  display: block;
  font-size: 0.58rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.35);
  margin-bottom: 1rem;
  padding: 0.4rem 2rem 0;
  border-top: 1px solid #222;
}

/* ── Grid ── */
.arts-grid {
  columns: 2;
  column-gap: 1rem;
  margin-bottom: 0;
  padding: 0 2rem 2rem;
}
@media (min-width: 640px) { .arts-grid { columns: 3; } }

.arts-item {
  break-inside: avoid;
  margin-bottom: 1rem;
  border: 2px solid #333;
  box-shadow: 4px 4px 0 #111;
  overflow: hidden;
  background: var(--m-beige);
  display: block;
  text-decoration: none;
  transition: transform 0.15s, box-shadow 0.15s;
}
.arts-item:hover {
  transform: translate(-2px,-2px);
  box-shadow: 6px 6px 0 #000;
}
.arts-item img {
  width: 100%;
  display: block;
  border-bottom: 1px solid #333;
  filter: saturate(0.75);
  transition: filter 0.3s;
}
.arts-item:hover img { filter: saturate(1.1); }
.arts-item-label {
  padding: 0.4rem 0.7rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.65rem;
  color: #555;
  letter-spacing: 0.05em;
}

.arts-footer-link {
  text-align: center;
  font-family: 'Righteous', sans-serif;
  font-size: 0.68rem;
  letter-spacing: 0.1em;
  color: rgba(255,255,255,0.3);
  padding: 0 2rem 0.5rem;
  border-top: 1px solid #222;
  padding-top: 1.2rem;
}
.arts-footer-link a {
  color: var(--mac-rose);
  text-decoration: none;
}

@media (max-width: 540px) {
  .arts-poster-ig { font-size: 0.65rem; bottom: 0.7rem; }
  .arts-section-label, .arts-works-label { padding-left: 1.2rem; }
  .arts-tags, .arts-grid { padding-left: 1.2rem; padding-right: 1.2rem; }
  .arts-footer-link { padding-left: 1.2rem; padding-right: 1.2rem; }
}
</style>

<div class="arts-page">

  <!-- Hero: Canva design as full image + Instagram link -->
  <div class="arts-hero">
    <img class="arts-hero-bg" src="/public/image/hero-arts-bg.jpg" alt="Cherainboow Arts — Creative Portfolio" />
    <a class="arts-poster-ig" href="https://www.instagram.com/cherainboow" target="_blank">↗ @cherainboow</a>
  </div>

  <!-- Quote -->
  <div class="arts-quote">
    <p>Wish to use <span class="qart">"Art"</span> to see the World<br>and <span class="qsci">"Science"</span> to color the Nature.</p>
    <cite>— Cherub</cite>
  </div>

  <!-- Media tags -->
  <span class="arts-section-label">— Mediums</span>
  <div class="arts-tags">
    <span class="arts-tag" style="background:var(--mac-rose)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--mac-lemon)">Watercolour</span>
    <span class="arts-tag" style="background:var(--mac-mint)">Acrylic</span>
    <span class="arts-tag" style="background:var(--mac-sky)">Procreate</span>
    <span class="arts-tag" style="background:var(--mac-lav)">Mixed Media</span>
    <span class="arts-tag" style="background:var(--m-warm)">Charcoal</span>
    <span class="arts-tag" style="background:var(--mac-peach)">Oil Pastel</span>
    <span class="arts-tag" style="background:var(--m-beige)">Illustration</span>
  </div>

  <!-- Works -->
  <span class="arts-works-label">— Works</span>
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

  <p class="arts-footer-link">
    More on <a href="https://www.instagram.com/cherainboow" target="_blank">@cherainboow</a>
  </p>

</div>
