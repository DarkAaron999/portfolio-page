---
layout: default
title: "3D Art"
---

<div class="page-header">
  <h1 class="project-title">🎮 3D Art</h1>
  <p class="project-subtitle">A collection of my 3D models. Click any card to view more details.</p>
</div>

<div class="project-grid">

  {% assign models = "woodenbarrel,fantasyplants,pinetree,sword,kitchen,alchemyhouse,factoryassets,rocks,deadtree,lgglogo" | split: "," %}

  {% for model in models %}
  <div class="project-card">
    <a href="{{ '/3dmodels/' | append: model | append: '.html' | relative_url }}">
      <img src="{{ '/assets/images/' | append: model | append: '.png' | relative_url }}">
      <div class="project-card-title">{{ model | replace: '-', ' ' | capitalize }}</div>
    </a>
  </div>
  {% endfor %}

</div>
