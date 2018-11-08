---
bg: "coke.jpg"
layout: page
permalink: /coke/
title: "coke"
crawlertitle: "Oduck84:Coke"
summary: "Cocacolra Collection"
active: Coke Play
---


{% for post in site.categories.coke limit:10 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}