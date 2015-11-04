---
title: Realise Blog
description: Read our blog
layout: default
hero-image: blog
hero-title: Realisers thoughts
hero-subtitle:
---
<div class="container">
    <ul>
        {% for post in site.posts %}
        <li>
            <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
            {{ post.excerpt }}
        </li>
        {% endfor %}
    </ul>
</div>