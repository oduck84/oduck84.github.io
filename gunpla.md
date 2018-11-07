---
bg: "gunpla.jpg"
layout: page
permalink: /gunpla/
title: "GUNPLA"
crawlertitle: "Oduck84:Gunpla"
summary: "건린이 건프라 도전기"
active: Gunpla
---


{% for post in site.categories.gunpla limit:10 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}