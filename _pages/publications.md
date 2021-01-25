---
layout: page
permalink: /publications/
title: publications
description: Here is a list of my publications sorted in reverse chronological order.
years: [2020, 2019, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
