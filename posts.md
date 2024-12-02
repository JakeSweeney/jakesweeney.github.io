---
layout: single
title: Blog Posts
---

{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{post.date | date: "%Y-%d-%m"}}</p>
<p>{{post.excerpt }}</p>
{% endfor %}