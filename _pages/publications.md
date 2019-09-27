---
layout: page
permalink: /publications/
title: publications
description: Publications by categories in reversed chronological order. Feel free to shoot me an email if you have questions.
years: [2019, 2018]
---

{% for y in page.years %}

  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
