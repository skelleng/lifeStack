---
layout: default
title: LifeStack – A Modular Philosophy for Intentional Living
permalink: /
---

# 🧬 LifeStack – A Modular Philosophy for Intentional Living

Welcome to LifeStack – a framework for intentional living built around three core layers:

- 🍳 [Cook](/cook/) – Nourish the body and mind
- 🧼 [Clean](/clean/) – Clear the clutter and cultivate clarity
- 🛠 [Build](/build/) – Create systems and shape the world

Each post is tagged and sorted into one of these pillars to help you explore the interconnected disciplines of health, clarity, and creation.

---

## 📝 All Posts

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
{% endfor %}
