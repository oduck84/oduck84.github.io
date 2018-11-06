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

  <div class="cover">

    <div class="cover-text">
      <div class="heading">

        {% if page.tags %}
          {% for tag in page.tags %}
            <a href="{{ site.baseurl }}/posts/#{{ tag | downcase }}">{{ tag | downcase }}</a>
          {% endfor %}
        {% else %}
          {{ page.title }}
        {% endif %}

      </div>

      <p>
        {% if page.summary %}
          {{ page.summary }}
        {% endif %}
      </p>

    </div>

  </div>

  </ul>

{% endfor %}
