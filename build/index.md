---
layout: default
title: Build
permalink: /build/
---

# 🛠 Build – Create Systems and Shape the World

{% assign posts = site.build | sort: 'date' | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
{% endfor %}
