---
layout: page
title: Task
permalink: /task/
order: 2
feature-img: "assets/img/pexels-pixabay-373543.jpg"
---

{% assign sorted_pages = site.pages | sort:"order" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}

