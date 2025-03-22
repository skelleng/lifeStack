---
layout: default
title: LifeStack – A Modular Philosophy for Intentional Living
permalink: /
---

{% include homepage-intro.html %}

---

## 📝 All Posts

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) 
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
{% endfor %}
