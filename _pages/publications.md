---
layout: page
permalink: /publications
title: Publications
description: Publications by categories in reversed chronological order. 
years: [2026, 2025, 2024, 2023]
nav: true
nav_rank: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>



