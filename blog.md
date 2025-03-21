---
layout: default
title: Blog
permalink: /blog/
---

# 📰 LifeStack Journal

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) <br>
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
{% endfor %}
