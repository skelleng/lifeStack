---
layout: default
title: LifeStack – A Modular Philosophy for Intentional Living
permalink: /
---
{% include homepage-intro.html %}
---

## 📝 All Posts

<div class="post-grid">
  {% assign posts = site.posts | sort: 'date' | reverse %}
  {% for post in posts %}
    <div class="post-card">
      <a href="{{ post.url | relative_url }}"><h3>{{ post.title }}</h3></a>
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      <div class="meta">
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
        <span class="readtime">
          {% assign words = post.content | number_of_words %}
          {% assign minutes = words | divided_by:200 | plus:1 %}
          ~{{ minutes }} min read
        </span>
      </div>
      {% if post.tags %}
        <div class="tags">
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
          {% endfor %}
        </div>
      {% endif %}
    </div>
  {% endfor %}
</div>
