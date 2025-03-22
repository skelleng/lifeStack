---
layout: default
title: LifeStack – A Modular Philosophy for Intentional Living
permalink: /
---

<nav style="padding: 1rem; background-color: #fff; font-family: sans-serif; font-size: 0.95rem; border-bottom: 1px solid #e0e0e0;">
  <a href="{{ '/' | relative_url }}" style="margin-right: 1rem; text-decoration: none; color: #333;">Home</a>
  <a href="{{ '/cook/' | relative_url }}" style="margin-right: 1rem; text-decoration: none; color: #333;">Cook</a>
  <a href="{{ '/clean/' | relative_url }}" style="margin-right: 1rem; text-decoration: none; color: #333;">Clean</a>
  <a href="{{ '/build/' | relative_url }}" style="margin-right: 1rem; text-decoration: none; color: #333;">Build</a>
  <a href="{{ '/about/' | relative_url }}" style="text-decoration: none; color: #333;">About</a>
</nav>

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
