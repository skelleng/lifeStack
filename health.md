---
layout: default
title: Health
permalink: /health/
tag: health
---

# 🌱 Health – Optimize Your Mind and Body

"Health" is about becoming physically strong, mentally sharp, and emotionally grounded. We explore everything from biohacking and breathwork to nutrition, supplements, fitness, and recovery.

## Key Themes
- Biohacking & wearables
- Sleep, recovery & optimization
- Fitness, routines, movement
- Nutrition & supplementation
- Mental wellness & mindfulness

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts %}
  {% if post.tags contains 'health' %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
  {% endif %}
{% endfor %}