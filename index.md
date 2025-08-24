---
layout: default
title: Beranda
---

<div class="grid">
  {% for post in site.posts %}
    <div class="card">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p><small>{{ post.date | date: "%d %B %Y" }}</small></p>
      <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
      <p><a href="{{ post.url | relative_url }}">Baca selengkapnya →</a></p>
    </div>
  {% endfor %}
</div>
