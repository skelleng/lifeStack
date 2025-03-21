---
layout: default
title: Cook
permalink: /cook/
---

# 🍳 Cook – Nourish the Body and Mind

{% assign sorted = site.cook | sort: 'date' | reverse %}
{% assign posts = site.cook | sort: 'date' | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
{% endfor %}
