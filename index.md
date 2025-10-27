---
layout: default
title: Home
---

# Welcome to Hive Mirror Blog

This is an automated mirror of posts from **@poprzeczka** on Hive.blog, translated to English.

## Latest Posts

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts %}
- **[{{ post.title }}]({{ post.url }})** - {{ post.date | date: "%B %d, %Y" }}
  - *By {{ post.author }}*
  - {{ post.description }}
{% endfor %}
