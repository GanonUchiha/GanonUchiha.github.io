---
layout: default
title: My Blog 📝
---

Welcome to my blog! Here are my latest posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>— {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
