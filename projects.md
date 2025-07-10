---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Welcome to my projects page! Here are some of my latest projects:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br />
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
