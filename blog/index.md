---
layout: default
title: My Blog 📝
---

Welcome to my blog! Here are my latest posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>
        — {{ post.date | date: "%B %d, %Y" }}
        {% if page.last_modified_at %}
            (Updated {{ page.last_modified_at | date: "%B %d, %Y" }})
        {% endif %}
      </small>
    </li>
  {% endfor %}
</ul>
