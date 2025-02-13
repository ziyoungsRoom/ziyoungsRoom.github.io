---
layout: default
title: Projects
---

<h1 class="detail-title">Projects.</h1>

<ul>
  {% for post in site.categories.projects %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> — {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
  {% endfor %}
</ul>
