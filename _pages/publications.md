---
layout: page
permalink: /publications/
title: publicaciones
description: publicaciones en orden cronológico inverso. generadas por jekyll-scholar.
years: [2021, 2020]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
