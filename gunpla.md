---
bg: "gunpla.jpg"
layout: page
permalink: /gunpla/
title: "Gunpla"
crawlertitle: "Gunpla"
summary: "Gunpla wold"
active: Gunpla
---


{% for post in site.categories.gunpla limit:10 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}