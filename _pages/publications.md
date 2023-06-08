---
layout: page
permalink: /publications/
title: publications
description: 
years: [2023, 2022, 2020, 2018, 2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

An up-to-date publication list can be found at [Google Scholar](https://scholar.google.com/citations?user=hmkEmtcAAAAJ).

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
