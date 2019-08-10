---
layout: page
title: Articles
permalink: /articles/
---

<ul>
{% for p in site.categories.article %}
  <h3><a href="{{ p.url }}">{{ p.title }}</a></h3>
  <p>{{ p.excerpt }}</p>
{% endfor %}
</ul>