---
layout: page
title: Blog
description: News and updates from EarHorn.
permalink: /blog/
---

{% if site.posts.size > 0 %}
{% for post in site.posts %}
<div class="card">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="text-muted">{{ post.date | date: "%B %-d, %Y" }}</p>
    {% if post.excerpt %}<p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>{% endif %}
</div>
{% endfor %}
{% else %}
*No posts yet. Check back soon.*
{% endif %}
