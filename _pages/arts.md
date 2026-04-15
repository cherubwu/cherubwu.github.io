---
layout: default
title: "CherainboowARTs"
permalink: /arts/
---

<link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;600;700&display=swap" rel="stylesheet">

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
  --dark:     #111009;
}

.arts-page {
  font-family: "PT Sans", Helvetica, sans-serif;
  color: var(--ink);
  max-width: 860px;
  margin: 0 auto;
  padding: 0 0 4rem;
}

/* ── Hero — black bg, multiply removes white ── */
.arts-hero {
  background: var(--dark);
  border: 3px solid var(--ink);
  box-shadow: 8px 8px 0 var(--ink);
  margin-bottom: 0;
  overflow: hidden;
  position: relative;
}
.arts-hero-bg {
  display: block;
  width: 100%;
  height: auto;
  mix-blend-mode: multiply;
  filter: saturate(1.4) contrast(1.1);
}
/* Title block below the illustration */
.arts-hero-text {
  background: var(--dark);
  padding: 1.4rem 2rem 1.8rem;
  border-top: 3px solid var(--ink);
  display: flex;
  flex-direction: column;
  gap: 0.45rem;
}
.arts-eyebrow {
  font-family: 'Caveat', cursive;
  font-size: 1rem;
  letter-spacing: 0.06em;
  color: var(--m-warm);
}
.arts-hero-name {
  font-family: 'Caveat', cursive;
  font-size: clamp(2.2rem, 5vw, 3.4rem);
  line-height: 1.0;
  color: #fff;
  margin: 0;
  font-weight: 700;
  letter-spacing: 0.02em;
}
.arts-hero-name span { color: var(--m-rose); }
.arts-hero-sub {
  font-family: 'Caveat', cursive;
  font-size: 1.05rem;
  color: var(--m-warm);
  line-height: 1.4;
  margin: 0;
}
.arts-hero-cta {
  display: inline-block;
  margin-top: 0.3rem;
  background: transparent;
  color: var(--m-rose) !important;
  padding: 0.45rem 1.2rem;
  font-family: 'Caveat', cursive;
  font-size: 1rem;
  letter-spacing: 0.06em;
  text-decoration: none;
  font-weight: 700;
  border: 2px solid var(--m-rose);
  box-shadow: 3px 3px 0 var(--m-rose);
  width: fit-content;
  transition: transform 0.15s, box-shadow 0.15s, background 0.15s;
}
.arts-hero-cta:hover {
  background: var(--m-rose);
  color: #fff !important;
  transform: translate(-2px,-2px);
  box-shadow: 5px 5px 0 var(--m-rose);
}

/* ── Quote ── */
.arts-quote {
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--m-rose);
  padding: 1.6rem 2rem;
  margin: 2.5rem 0 2.5rem;
  background: var(--m-beige);
  position: relative;
}
.arts-quote p {
  font-family: 'Caveat', cursive;
  font-size: 1.3rem;
  line-height: 1.5;
  color: var(--ink);
  margin: 0 0 0.4rem;
}
.arts-quote p em { color: var(--m-terra); font-style: normal; font-weight: 700; }
.arts-quote cite {
  font-size: 0.62rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--m-warm);
  font-family: "PT Sans", sans-serif;
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

/* ── Medium tags ── */
.arts-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 2rem;
}
.arts-tag {
  padding: 0.28rem 0.85rem;
  font-family: 'Caveat', cursive;
  font-size: 0.95rem;
  font-weight: 600;
  border: 2px solid var(--ink);
  color: var(--ink);
  letter-spacing: 0.03em;
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
  filter: saturate(0.7);
}
.arts-item:hover img { filter: saturate(1.15); }
.arts-item-label {
  padding: 0.45rem 0.75rem;
  font-family: 'Caveat', cursive;
  font-size: 0.9rem;
  color: var(--m-warm);
  font-weight: 600;
  background: var(--m-beige);
}

@media (max-width: 600px) {
  .arts-hero-bg { min-height: 200px; object-fit: contain; }
}
</style>

<div class="arts-page">

  <!-- Hero: illustration on black, title below -->
  <div class="arts-hero">
    <img class="arts-hero-bg" src="/public/image/hero-arts.png" alt="Cherainboow Arts" />
    <div class="arts-hero-text">
      <span class="arts-eyebrow">— Visual Portfolio</span>
      <div class="arts-hero-name">Cherainboow<span>ARTs</span></div>
      <p class="arts-hero-sub">Portrait · Landscape · Watercolour · Acrylic · Mixed Media<br>Procreate · Pencil & Charcoal · Oil Pastel · Illustration</p>
      <a class="arts-hero-cta" href="https://www.instagram.com/cherainboow" target="_blank">↗ Follow on Instagram</a>
    </div>
  </div>

  <!-- Quote -->
  <div class="arts-quote">
    <p>Wish to use <em>"Art"</em> to see the World<br>and <em>"Science"</em> to color the Nature.</p>
    <cite>— Cherub</cite>
  </div>

  <!-- Works -->
  <span class="arts-section-label">— Works</span>
  <div class="arts-tags">
    <span class="arts-tag" style="background:var(--m-rose)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--m-beige)">Watercolour</span>
    <span class="arts-tag" style="background:var(--m-sage)">Acrylic</span>
    <span class="arts-tag" style="background:var(--m-blue)">Procreate</span>
    <span class="arts-tag" style="background:var(--m-lav)">Mixed Media</span>
    <span class="arts-tag" style="background:var(--m-warm)">Charcoal</span>
    <span class="arts-tag" style="background:var(--m-terra)">Oil Pastel</span>
  </div>

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

  <p style="text-align:center;font-family:'Caveat',cursive;font-size:1rem;color:var(--m-warm);">
    More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:var(--m-rose);text-decoration:none;font-weight:700;">@cherainboow</a>
  </p>

</div>
