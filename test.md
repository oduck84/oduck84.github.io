---
bg: "tag.jpg"
layout: page
permalink: /postss/
title: "test"
crawlertitle: "All test"
summary: "Posts about jekyll"
active: archive
---


{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}


  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>

  <ul class="year">
    <main class="content-wrapper">
      {{ content }}
    </main>

    {% include footer.html %}
  </ul>



{% endfor %}
