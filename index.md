---
layout: default
title: Home
---

<!-- HERO -->
<div class="hero text-center">
  <h1>Welcome to the 61st District Court</h1>
  <p>Achieving excellence, accountability, and transparency in our judiciary</p>
</div>

<!-- QUICK‑ACTION TILES -->
<div class="tile‑row">
  {% assign tiles = "Case Lookup,Pay Fines & Fees,Daily Dockets,Contact Us" | split: ',' %}
  {% assign icons = "search,credit-card,calendar,mailbox" | split: ',' %}
  {% for tile in tiles %}
    <a href="#" class="quick-tile">
      <i class="bi bi-{{ icons[forloop.index0] }}"></i>
      <span class="d-block mt‑2">{{ tile }}</span>
    </a>
  {% endfor %}
</div>

<!-- THREE CARD SECTIONS -->
<div class="section‑grid">

  <section class="card">
    <h2>Case Types</h2>
    <ul>
      <li><a href="#">Criminal</a></li>
      <li><a href="#">Traffic</a></li>
      <li><a href="#">Civil</a></li>
    </ul>
  </section>

  <section class="card">
    <h2>Online Services</h2>
    <ul>
      <li><a href="#">Case Lookup</a></li>
      <li><a href="#">Pay Fines & Fees</a></li>
      <li><a href="#">Daily Dockets</a></li>
    </ul>
  </section>

  <section class="card">
    <h2>News & Announcements</h2>
    <ul>
      <li><a href="#">Press Release</a></li>
      <li><a href="#">March 28 2024</a></li>
    </ul>
  </section>

</div>

<!-- BIG BUTTON STRIP -->
<div class="big‑btn‑row">
  <a href="#" class="big‑btn">Juror Information</a>
  <a href="#" class="big‑btn">Forms & Resources</a>
  <a href="#" class="big‑btn">Probation Services</a>
</div>
