---
layout: default
title: Cook
permalink: /cook/
---

# 🍳 Cook – Nourish the Body and Mind

{% assign sorted = site.cook | sort: 'date' | reverse %}
{% for post in sorted %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small>
  {% if post.tags %}
    <br><small>Tags: 
    {% for tag in post.tags %}
      <a href="/tag/{{ tag | slugify }}/">{{ tag }}</a>{% if forloop.last == false %}, {% endif %}
    {% endfor %}
    </small>
  {% endif %}
  <br><br>
{% endfor %}
