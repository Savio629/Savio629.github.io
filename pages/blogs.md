---
layout: blogs
title: Blogs
permalink: /blogs/
pagination:
  enabled: true
  collection: blogs
---

{% for blog in paginator.posts %}
    <div>
        <a href="{{ blog.permalink }}">
            <h3>{{ blog.title }}</h3>
        </a>
        <div>{{ blog.description }}</div>
    </div>
{% endfor %}

{% include pagination.html %}
