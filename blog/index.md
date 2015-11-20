---
title: Realise Blog
description: Read our blog
layout: default
hero-image: blog
hero-title: Realisers' thoughts
hero-subtitle:
---
<div class="blog-container">
{% for post in site.posts %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <h4>{{ post.author }} &bull; {{ post.date | date: "%B %-d, %Y" }}</h4>
    {% if post.teaser %}<p>{{ post.teaser }}</p>{% else %}
    <p>{{ post.content | strip_html | truncatewords: 20 }}</p>{% endif %}
    <p><a href="{{ post.url }}">Read more</a></p>
{% endfor %}
</div>