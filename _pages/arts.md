---
layout: page
title: "CherainboowARTs"
permalink: /arts/
---

<style>
/* ── Portfolio Page ── */
.portfolio-hero {
  margin: -1rem -1rem 3rem;
  padding: 4rem 2rem 3rem;
  background: #1a1a1a;
  text-align: center;
  position: relative;
  overflow: hidden;
}
.portfolio-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    45deg,
    transparent,
    transparent 40px,
    rgba(255,255,255,0.02) 40px,
    rgba(255,255,255,0.02) 80px
  );
}
.portfolio-hero h2 {
  font-family: "Abril Fatface", serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  color: #fff;
  margin: 0 0 0.5rem;
  letter-spacing: -0.02em;
  position: relative;
  border: none;
}
.portfolio-hero h2 span {
  color: #aa759f;
}
.portfolio-hero p {
  color: rgba(255,255,255,0.5);
  font-size: 0.85rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  position: relative;
  margin: 0 0 1.5rem;
}
.portfolio-hero a.ig-btn {
  display: inline-block;
  background: linear-gradient(135deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
  color: #fff !important;
  padding: 0.6rem 1.6rem;
  border-radius: 2px;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  text-decoration: none;
  font-weight: 700;
  position: relative;
  transition: opacity 0.2s;
}
.portfolio-hero a.ig-btn:hover { opacity: 0.85; }

/* Grid */
.portfolio-grid {
  columns: 2;
  column-gap: 1rem;
  margin-bottom: 3rem;
}
@media (min-width: 48em) {
  .portfolio-grid { columns: 3; }
}
.portfolio-item {
  break-inside: avoid;
  margin-bottom: 1rem;
  position: relative;
  overflow: hidden;
  background: #111;
}
.portfolio-item img {
  width: 100%;
  display: block;
  transition: transform 0.4s ease, filter 0.4s ease;
  filter: saturate(0.85);
}
.portfolio-item:hover img {
  transform: scale(1.04);
  filter: saturate(1.2);
}
.portfolio-item-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(to top, rgba(0,0,0,0.6) 0%, transparent 50%);
  opacity: 0;
  transition: opacity 0.3s;
  display: flex;
  align-items: flex-end;
  padding: 1rem;
}
.portfolio-item:hover .portfolio-item-overlay { opacity: 1; }
.portfolio-item-title {
  color: #fff;
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

/* Quote */
.portfolio-quote {
  border-left: 4px solid #aa759f;
  padding: 1rem 1.5rem;
  margin: 2rem 0 3rem;
  background: rgba(170, 117, 159, 0.06);
}
.portfolio-quote p {
  font-family: "Abril Fatface", serif;
  font-size: 1.1rem;
  color: #555;
  margin: 0 0 0.3rem;
  line-height: 1.5;
}
.portfolio-quote cite {
  font-size: 0.72rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: #aa759f;
}
</style>

<div class="portfolio-hero">
  <h2>Cherainboow<span>ARTs</span></h2>
  <p>Painting · Photography · Visual Stories</p>
  <a href="https://www.instagram.com/cherainboow" target="_blank" class="ig-btn">↗ Follow on Instagram</a>
</div>

<div class="portfolio-quote">
  <p>"To see a World in a Grain of Sand, and a Heaven in a Wild Flower."</p>
  <cite>— William Blake</cite>
</div>

<div class="portfolio-grid">

  <div class="portfolio-item">
    <img src="/public/image/Oilp.JPG" alt="Oil Painting" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">Oil Painting</span>
    </div>
  </div>

  <div class="portfolio-item">
    <img src="/public/image/Evergreen.JPG" alt="Evergreen" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">Evergreen</span>
    </div>
  </div>

  <div class="portfolio-item">
    <img src="/public/image/KAEO.PNG" alt="KAEO" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">KAEO</span>
    </div>
  </div>

  <div class="portfolio-item">
    <img src="/public/image/abg.JPG" alt="Abstract" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">Abstract</span>
    </div>
  </div>

  <div class="portfolio-item">
    <img src="/public/image/scottish-fantazy-cover.png" alt="Scottish Fantasy" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">Scottish Fantasy</span>
    </div>
  </div>

  <div class="portfolio-item">
    <img src="/public/image/candy.png" alt="Candy" />
    <div class="portfolio-item-overlay">
      <span class="portfolio-item-title">Candy</span>
    </div>
  </div>

</div>

<p style="text-align:center; font-size:0.75rem; letter-spacing:0.16em; text-transform:uppercase; color:#aaa;">
  More on <a href="https://www.instagram.com/cherainboow" target="_blank" style="color:#aa759f;">@cherainboow</a>
</p>
