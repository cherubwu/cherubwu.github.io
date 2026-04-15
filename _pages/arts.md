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
  --dark:     #0d0d0d;
}

.arts-page {
  font-family: "PT Sans", sans-serif;
  color: var(--ink);
  max-width: 860px;
  margin: 0 auto;
  padding: 0 0 4rem;
}

/* ── Hero ── */
.arts-hero {
  background: var(--dark);
  border: 3px solid #333;
  box-shadow: 8px 8px 0 #333;
  margin-bottom: 2.5rem;
  overflow: hidden;
  position: relative;
}
.arts-hero-illus {
  display: block;
  width: 100%;
  height: auto;
  mix-blend-mode: multiply;
  filter: saturate(1.35) contrast(1.05);
  position: relative;
  z-index: 1;
}

/* ── Poster title overlay ── */
.arts-poster {
  background: var(--dark);
  padding: 1.6rem 2rem 2rem;
  position: relative;
  z-index: 2;
  border-top: 2px solid #222;
}
.arts-poster-line {
  display: block;
  line-height: 1;
  margin-bottom: 0.5rem;
}
.arts-poster-line:last-child { margin-bottom: 0; }

/* ── Highlight word blocks ── */
.hw {
  display: inline-block;
  font-family: 'Pacifico', cursive;
  padding: 0.1em 0.25em;
  line-height: 1.05;
  position: relative;
}
.hw-sm {
  font-family: 'Righteous', sans-serif;
  font-size: 0.55em;
  letter-spacing: 0.06em;
  display: inline-block;
  vertical-align: middle;
  color: var(--m-warm);
  padding: 0 0.3em;
}

.hw-cherainboow {
  font-size: clamp(2.4rem, 6vw, 4.2rem);
  background: var(--m-lav);
  color: var(--dark);
  transform: rotate(-1.2deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.4);
}
.hw-arts {
  font-size: clamp(2.8rem, 7vw, 5rem);
  background: var(--m-rose);
  color: #fff;
  transform: rotate(0.8deg);
  box-shadow: 4px 4px 0 rgba(0,0,0,0.4);
  margin-left: 0.2em;
}
.hw-art {
  font-size: clamp(1.6rem, 3.5vw, 2.6rem);
  background: var(--m-terra);
  color: #fff;
  transform: rotate(-0.5deg);
  box-shadow: 3px 3px 0 rgba(0,0,0,0.3);
}
.hw-science {
  font-size: clamp(1.6rem, 3.5vw, 2.6rem);
  background: var(--m-sage);
  color: var(--dark);
  transform: rotate(1deg);
  box-shadow: 3px 3px 0 rgba(0,0,0,0.3);
  margin-left: 0.15em;
}
.hw-plain {
  font-family: 'Righteous', sans-serif;
  font-size: clamp(1rem, 2vw, 1.5rem);
  color: rgba(255,255,255,0.55);
  padding: 0;
  letter-spacing: 0.04em;
}

.arts-poster-ig {
  margin-top: 1.2rem;
  display: inline-block;
  background: transparent;
  color: var(--m-rose) !important;
  padding: 0.4rem 1.1rem;
  font-family: 'Righteous', sans-serif;
  font-size: 0.82rem;
  letter-spacing: 0.08em;
  text-decoration: none;
  border: 2px solid var(--m-rose);
  box-shadow: 3px 3px 0 var(--m-rose);
  transition: transform 0.15s, box-shadow 0.15s, background 0.15s;
}
.arts-poster-ig:hover {
  background: var(--m-rose);
  color: #fff !important;
  transform: translate(-2px,-2px);
  box-shadow: 5px 5px 0 var(--m-rose);
}

/* ── Quote ── */
.arts-quote {
  border: 2.5px solid var(--ink);
  box-shadow: 5px 5px 0 var(--m-rose);
  padding: 1.5rem 1.8rem;
  margin-bottom: 2.5rem;
  background: var(--m-beige);
}
.arts-quote p {
  font-family: 'Pacifico', cursive;
  font-size: clamp(1rem, 2.2vw, 1.3rem);
  line-height: 1.6;
  color: var(--ink);
  margin: 0 0 0.4rem;
}
.arts-quote p .qem { color: var(--m-terra); }
.arts-quote cite {
  font-size: 0.6rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--m-warm);
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
  font-size: 0.72rem;
  font-weight: 400;
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
</style>

<div class="arts-page">

  <!-- Hero -->
  <div class="arts-hero">
    <img class="arts-hero-illus" src="/public/image/hero-arts.png" alt="Cherainboow Arts" />
    <div class="arts-poster">
      <span class="arts-poster-line">
        <span class="hw hw-cherainboow">Cherainboow</span>
        <span class="hw hw-arts">ARTs</span>
      </span>
      <span class="arts-poster-line" style="margin-top:0.6rem">
        <span class="hw hw-plain">wish to use </span>
        <span class="hw hw-art">"Art"</span>
        <span class="hw hw-plain"> to see the World</span>
      </span>
      <span class="arts-poster-line">
        <span class="hw hw-plain">and </span>
        <span class="hw hw-science">"Science"</span>
        <span class="hw hw-plain"> to color the Nature</span>
      </span>
      <div>
        <a class="arts-poster-ig" href="https://www.instagram.com/cherainboow" target="_blank">↗ @cherainboow</a>
      </div>
    </div>
  </div>

  <!-- Media tags -->
  <span class="arts-section-label">— Mediums</span>
  <div class="arts-tags">
    <span class="arts-tag" style="background:var(--m-rose)">Oil Painting</span>
    <span class="arts-tag" style="background:var(--m-beige)">Watercolour</span>
    <span class="arts-tag" style="background:var(--m-sage)">Acrylic</span>
    <span class="arts-tag" style="background:var(--m-blue)">Procreate</span>
    <span class="arts-tag" style="background:var(--m-lav)">Mixed Media</span>
    <span class="arts-tag" style="background:var(--m-warm)">Charcoal</span>
    <span class="arts-tag" style="background:var(--m-terra);color:#fff">Oil Pastel</span>
    <span class="arts-tag" style="background:var(--m-beige)">Illustration</span>
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
    More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:var(--m-rose);text-decoration:none;">@cherainboow</a>
  </p>

</div>
