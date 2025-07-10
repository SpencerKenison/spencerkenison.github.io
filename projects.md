---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Here are some of my latest projects:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br />
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

## GitHub Repositories

<ul>
  {% for repo in site.github.public_repos %}
    <li>
      <a href="{{ repo.html_url }}" target="_blank">{{ repo.name }}</a>
      {% if repo.description %}
        - {{ repo.description }}
      {% endif %}
    </li>
  {% endfor %}
</ul>

---
