---
layout: archive
permalink: /blogs/index.html
title: Blogs
author_profile: true
---

### 2025

{% assign year_posts = site.posts | where_exp:"post","post.date >= '2025-01-01' and post.date < '2026-01-01'" %}
<ul>
  {% for post in year_posts %}
    {% if post.path contains 'blogs/' %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> <span>({{ post.date | date: "%Y-%m-%d" }})</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

<br>

## Leave a Message

<br>

{% include disqus.html %} 

<br>
