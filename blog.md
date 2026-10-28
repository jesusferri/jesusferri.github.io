---
layout: default
title: Blog de SEO
description: Noticias, novedades de Google y guías prácticas de SEO.
permalink: /blog/
---
# Blog de SEO

<p class="lead">Noticias, cambios de Google y guías prácticas.</p>

<ul class="posts">
{% for post in site.posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  <p class="meta">{{ post.date | date: "%d/%m/%Y" }}</p>
  <p>{{ post.description }}</p></li>
{% endfor %}
</ul>
