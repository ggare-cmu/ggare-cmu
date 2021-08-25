---
layout: page
permalink: /publications/
title: Publications
description: The recent updated list is available on <a href="https://scholar.google.co.in/citations?hl=en&user=BX4jUxEAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar</a>
years: [2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
