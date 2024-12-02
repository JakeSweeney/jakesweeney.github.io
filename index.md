---
layout: single
title: Home Page
---
## Latest Website Updates
{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{post.date | date: "%Y-%d-%m"}}</p>
<p>{{post.excerpt }}</p>
{% endfor %}

## Pinned Items
