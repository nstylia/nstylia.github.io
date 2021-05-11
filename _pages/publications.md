---
layout: page
permalink: /publications/
title: publications
description: For detailed citation information please check my <a href="https://scholar.google.com/citations?user=l1IYDIUAAAAJ">Google Scholar</a> page.
years: [2021, 2020, 2019, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
