---
title: Dev Notes on Power Platform
---

<div class="timeline-container">
  {% for post in site.posts %}
  <div class="timeline-item">
    <div class="timeline-dot"></div>
    <div class="timeline-content">
      <span class="post-date">Updated {{ post.date | date: "%b %d, %Y" }}</span>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    </div>
  </div>
  {% endfor %}
</div>
