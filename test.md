---
bg: "gunpla.jpg"
layout: page
permalink: /test/
title: "한글테스트2"
crawlertitle: "한글테스트3"
summary: "한글테스트4"
active: Gunpla
---


{% for post in site.categories.gunpla limit:10 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}