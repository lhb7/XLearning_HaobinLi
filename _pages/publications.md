---
layout: page
permalink: /Publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [2021]
nav: true
---

### Interests
My research lies in the field of Computer Vision and Deep Learning. For now I focus on the subspace learning and clustering, which can be unified to the framework of Representation Learning.

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
