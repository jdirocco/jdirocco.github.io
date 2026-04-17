---
layout: page
permalink: /publications/
title: Publications
description: Complete list of publications. See also <a style="color:green" href="https://dblp.uni-trier.de/pid/145/3999.html">[DBLP]</a>, <a style="color:green" href="https://scholar.google.com/citations?user=PNagLbIAAAAJ&hl=it&oi=ao">[Google Scholar]</a>, <a style="color:green" href="https://orcid.org/0000-0002-2954-5289">[ORCID]</a>, <a style="color:green" href="https://www.scopus.com/authid/detail.uri?authorId=55877197500">[Scopus]</a>.
years: [2026, 2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
