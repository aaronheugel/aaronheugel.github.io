---
layout: default
title: Home
---

Welcome. I’m a writer based in Queens. My work explores the quiet intersections of place, memory, and the everyday — through essays, poetry, and longer reflections.

## Recent Writing

{% include post-list.html limit=5 empty_message="New writing will appear here soon." %}

{% if site.posts.size > 5 %}
<p class="all-writing-link"><a href="{{ '/writing/' | relative_url }}">All writing &rarr;</a></p>
{% endif %}
