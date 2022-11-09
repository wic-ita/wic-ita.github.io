---
layout: page
title: Important Dates
permalink: /dates/
order: 4
feature-img: "assets/img/pexels-pawe-l-1309687.jpg"
---

{% assign sorted_pages = site.pages | sort:"order" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}


**Development Data Release**: February 7th, 2023

**Registration closes**: April 30th, 2023

**Evaluation window**: May 2nd-19th, 2023

**Results ranking**: May 30th, 2023

**Final report submission**: June 14th, 2023

**Camera-ready version deadline**: July 25th, 2023

**EVALITA 2023**: September 7th-8th, 2023

