---
title: Abby Kong's Dev Notes on Power Platform
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> — {{ post.date | date_to_string }}</span>
    </li>
  {% endfor %}
</ul>
This blog site is generated from Git Hub Pages
