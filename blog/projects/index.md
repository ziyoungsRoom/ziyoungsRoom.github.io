---
layout: default
title: Projects
---

<h1 class="list-title">Projects.</h1>

<ul>
  {% for post in site.categories.projects %}
  <li class='post-card'>
    <a href="{{ post.url | relative_url }}"> 
      <h2 class='post-title'>{{ post.title }} </h2>
      <div class="excerpt">{{ post.excerpt }}</div>
      <div class='post-date'>{{ post.date | date: "%Y년 %m월 %d일" }}</div>
    </a>
  </li>
  {% endfor %}
</ul>
