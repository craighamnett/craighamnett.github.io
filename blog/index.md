---
title: Realise Blog
layout: default
description: Read our blog
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>