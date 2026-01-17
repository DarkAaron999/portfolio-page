---
layout: default
title: "Design Week"
---

<div class="page-header">
  <h1 class="project-title">🧩 Design Week</h1>
  <p class="project-subtitle">A series of rapid design challenges exploring level design, iteration, and collaboration.</p>
</div>

<div class="project-grid">

  {% assign weeks = "designweek01,designweek02,designweek03,designweek04,designweek05,designweek06" | split: "," %}

  {% for week in weeks %}
  <div class="project-card">
    <a href="{{ '/designweek/' | append: week | append: '.html' | relative_url }}">
      <img src="{{ '/assets/images/' | append: week | append: '.png' | relative_url }}">
      <div class="project-card-title">{{ week | replace: 'designweek', 'Design Week ' }}</div>
    </a>
  </div>
  {% endfor %}

</div>
