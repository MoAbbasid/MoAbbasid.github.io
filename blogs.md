---
layout: archive
permalink: /blogs/index.html
title: Blogs
author_profile: true
---

### Blog Posts

{% assign blog_pages = site.pages | where_exp:"page","page.path contains 'blogs/'" | where_exp:"page","page.path != 'blogs.md'" | sort: "date" | reverse %}
<ul>
  {% for blog in blog_pages %}
    {% if blog.title and blog.url %}
      <li>
        <a href="{{ blog.url }}">{{ blog.title }}</a>{% if blog.date %} <span>({{ blog.date | date: "%Y-%m-%d" }})</span>{% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>

<br>

## Leave a Message

<br>

{% include disqus.html %} 

<br>
