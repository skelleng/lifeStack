---
layout: default
title: Wealth
permalink: /wealth/
tag: wealth
---

# 💸 Wealth – Build Systems That Grow

"Wealth" is about building personal freedom through smart systems. Whether you're automating income, mastering crypto, or exploring the latest tools, this pillar focuses on creating value and scaling impact.

## Key Themes
- AI tools for creators
- Crypto, DeFi & trading
- Affiliate marketing strategies
- Investing & personal finance
- Passive income & solopreneurship

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts %}
  {% if post.tags contains 'wealth' %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small><br><br>
  {% endif %}
{% endfor %}