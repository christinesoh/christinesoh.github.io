---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2021, 2019]
pres_years: [2021, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div class="publications">

<p> Presentations</p>

{% for y in page.pres_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}


</div>
