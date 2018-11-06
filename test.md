---
bg: "tag.jpg"
layout: page
permalink: /postss/
title: "test13"
crawlertitle: "All test"
summary: "Posts about jekyll"
active: archive
---



{% for post in site.posts limit: 10%}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
S