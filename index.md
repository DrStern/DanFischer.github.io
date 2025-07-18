---
layout: default
title: Home
---

<div class="hero text-center">
  <div class="container">
    <h1>Welcome to the 61st District Court</h1>
    <p class="lead">Achieving excellence, accountability, and transparency in our judiciary</p>
  </div>
</div>

<!-- QUICK‑ACTION TILES -->
<div class="container my-5">
  <div class="row text-center g-4">
    {% assign tiles = "Case Lookup,Pay Fines & Fees,Daily Dockets,Contact Us" | split: ',' %}
    {% assign icons = "search,credit-card,calendar,mailbox" | split: ',' %}
    {% for tile in tiles %}
      <div class="col-6 col-md-3">
        <a href="#" class="d-block quick-tile py-4 text-decoration-none text-dark">
          <i class="bi bi-{{ icons[forloop.index0] }} fs-1 mb-2"></i>
          <h6 class="m-0">{{ tile }}</h6>
        </a>
      </div>
    {% endfor %}
  </div>
</div>

<!-- THREE COLUMNS -->
<div class="container my-5">
  <div class="row g-4">
    <div class="col-md">
      <h5>Case Types</h5>
      <ul class="list-unstyled">
        <li>Criminal</li><li>Traffic</li><li>Civil</li>
      </ul>
    </div>
    <div class="col-md">
      <h5>Online Services</h5>
      <ul class="list-unstyled">
        <li>Case Lookup</li><li>Pay Fines & Fees</li><li>Daily Dockets</li>
      </ul>
    </div>
    <div class="col-md">
      <h5>News & Announcements</h5>
      <ul class="list-unstyled">
        <li>Press Release</li><li>March 28, 2024</li>
      </ul>
    </div>
  </div>
</div>

<!-- BIG BUTTON STRIP -->
<div class="container mb-5">
  <div class="row g-3">
    <div class="col-md"><a href="#" class="btn btn-primary big-btn">Juror Information</a></div>
    <div class="col-md"><a href="#" class="btn btn-primary big-btn">Forms & Resources</a></div>
    <div class="col-md"><a href="#" class="btn btn-primary big-btn">Probation Services</a></div>
  </div>
</div>
