---
layout: default
title: "CherainboowARTs"
permalink: /arts/
---

<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Righteous&family=PT+Sans:wght@400;700&display=swap" rel="stylesheet">

<style>
:root {
  --m-beige:  #E8E2D7;
  --m-rose:   #C9A9A6;
  --m-sage:   #8FAF8A;
  --m-blue:   #8BA7B8;
  --m-terra:  #C4846A;
  --m-lav:    #A89BB0;
  --m-warm:   #B5AFA8;
  --ink:      #2C2C2C;
  /* Candy colors */
  --candy-pink:   #FF6EB4;
  --candy-cyan:   #3DD9DC;
  --candy-yellow: #FFE44D;
  --candy-mint:   #5CEFC7;
  --candy-lav:    #C084FC;
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
  box-shadow: 8px 8px 0 #1a1a1a;
  margin-bottom: 2.5rem;
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
  object-position: center top;
}

/* Dark gradient only on left-bottom so title is readable */
.arts-hero-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    to right,
    rgba(10,10,10,0.72) 0%,
    rgba(10,10,10,0.4) 40%,
    rgba(10,10,10,0.0) 65%
  ),
  linear-gradient(
    to top,
    rgba(10,10,10,0.7) 0%,
    rgba(10,10,10,0.1) 40%,
    transparent 70%
  );
}

/* Title pinned to bottom-left */
.arts-poster {
  position: absolute;
  bottom: 1.6rem;
  left: 1.8rem;
  z-index: 3;
  display: flex;
  flex-direction: column;
  gap: 0.3rem;
}

.hw {
  display: inline-block;
  font-family: 'Pacifico', cursive;
  line-height: 1.05;
  padding: 0.06em 0.22em;
  position: relative;
}
.hw-cherainboow {
  font-size: clamp(1.8rem, 4vw, 3rem);
  background: var(--candy-pink);
  color: #fff;
  transform: rotate(-1.5deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.5);
}
.hw-arts {
  font-size: clamp(2.2rem, 5vw, 3.8rem);
  background: var(--candy-cyan);
  color: #0d0d0d;
  transform: rotate(1deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.5);
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
  color: var(--candy-yellow) !important;
  padding: 0.35rem 1rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-decoration: none;
  border: 2px solid var(--candy-yellow);
  box-shadow: 3px 3px 0 var(--candy-yellow);
  width: fit-content;
  transition: transform 0.15s, box-shadow 0.15s, background 0.15s;
}
.arts-poster-ig:hover {
  background: var(--candy-yellow);
  color: #0d0d0d !important;
  transform: translate(-2px,-2px);
  box-shadow: 5px 5px 0 var(--candy-yellow);
}

/* ── Quote ── */
.arts-quote {
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--candy-pink);
  padding: 1.5rem 1.8rem;
  margin-bottom: 2.5rem;
  background: #0d0d0d;
}
.arts-quote p {
  font-family: 'Pacifico', cursive;
  font-size: clamp(1rem, 2vw, 1.2rem);
  line-height: 1.65;
  color: #fff;
  margin: 0 0 0.4rem;
}
.arts-quote p .qart { color: var(--candy-pink); }
.arts-quote p .qsci { color: var(--candy-cyan); }
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
  .arts-hero { min-height: 280px; }
  .arts-poster { bottom: 1rem; left: 1rem; }
}
</style>

<div class="arts-page">

  <!-- Hero: illustration + gradient overlay + title bottom-left -->
  <div class="arts-hero">
    <img class="arts-hero-bg" src="/public/image/hero-arts.png" alt="Cherainboow Arts" />
    <div class="arts-hero-overlay"></div>
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
    <span class="arts-tag" style="background:var(--candy-pink);border-color:var(--ink)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--candy-yellow);border-color:var(--ink)">Watercolour</span>
    <span class="arts-tag" style="background:var(--candy-mint);border-color:var(--ink)">Acrylic</span>
    <span class="arts-tag" style="background:var(--candy-cyan);border-color:var(--ink)">Procreate</span>
    <span class="arts-tag" style="background:var(--candy-lav);border-color:var(--ink);color:#fff">Mixed Media</span>
    <span class="arts-tag" style="background:var(--m-warm);border-color:var(--ink)">Charcoal</span>
    <span class="arts-tag" style="background:var(--m-terra);border-color:var(--ink);color:#fff">Oil Pastel</span>
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
    More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:var(--candy-pink);text-decoration:none;">@cherainboow</a>
  </p>

</div>
