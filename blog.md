---
layout: default
title: Blog
---

<h1>📚 Blog</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
      <span> — {{ post.date | date: "%Y.%m.%d" }}</span>
    </li>
  {% endfor %}
</ul>
