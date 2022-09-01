---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2020, 2021, 2022]
nav: false
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
