---
layout: page
permalink: /publications/
title: publications
years: [2027, 2026, 2025, 2024, 2023, 2022, 2021, 2019, 2018]
---

<h3>Preprints</h3>

{% for y in page.years %}
  {% bibliography -f preprint_papers -q @*[year={{y}}]* %}
{% endfor %}

<h3>Conference Papers</h3>

{% for y in page.years %}
  {% bibliography -f conference_papers -q @*[year={{y}}]* %}
{% endfor %}
