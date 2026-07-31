---
layout: default
title: Home
---

Welcome. I’m a writer based in Queens. My work explores the quiet intersections of place, memory, and the everyday — through essays, poetry, and longer reflections.

## Recent Writing

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
      {% if post.excerpt %}
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% if site.posts.size == 0 %}
  <p>New writing will appear here soon.</p>
{% endif %}
