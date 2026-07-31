---
layout: default
title: Writing
permalink: /writing/
---

# Writing

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
      {% if post.excerpt %}
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% if site.posts.size == 0 %}
  <p>No pieces published yet. Check back soon.</p>
{% endif %}
