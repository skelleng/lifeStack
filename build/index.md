---
layout: default
title: Build
permalink: /build/
---

# 🍳 Build – Create

{% assign sorted = site.build | sort: 'date' | reverse %}
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
