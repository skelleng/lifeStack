---
layout: default
title: Clean
permalink: /clean/
---

# 🍳 Clean – Sustain

{% assign sorted = site.clean| sort: 'date' | reverse %}
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
