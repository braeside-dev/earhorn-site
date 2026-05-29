---
layout: page
title: Blog
description: News and updates from EarHorn.
permalink: /blog/
---

{% if site.posts.size > 0 %}
{% for post in site.posts %}
{% comment %} Card image: use an explicit `image:` in front matter if set, otherwise grab the first <img> from the post body automatically. {% endcomment %}
{% assign card_image = nil %}
{% assign card_image_alt = post.image_alt %}
{% if post.image %}
    {% assign card_image = post.image | relative_url %}
{% elsif post.content contains '<img' %}
    {% assign img_tag = post.content | split: '<img ' | last %}
    {% assign card_image = img_tag | split: 'src="' | last | split: '"' | first %}
    {% if img_tag contains 'alt="' %}{% assign card_image_alt = img_tag | split: 'alt="' | last | split: '"' | first %}{% endif %}
{% endif %}
<div class="card">
    {% if card_image %}<a href="{{ post.url | relative_url }}" class="card-image"><img src="{{ card_image }}" alt="{{ card_image_alt }}" loading="lazy"></a>{% endif %}
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="text-muted">{{ post.date | date: "%B %-d, %Y" }}</p>
    {% if post.excerpt %}<p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>{% endif %}
</div>
{% endfor %}
{% else %}
*No posts yet. Check back soon.*
{% endif %}
