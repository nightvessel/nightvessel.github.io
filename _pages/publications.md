---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2020,2019,2016,2015]
nav: true
---

For a full publication list: [Google Scholar](https://scholar.google.com/citations?user=rRlIHi4AAAAJ&hl=en)

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
