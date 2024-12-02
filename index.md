---
layout: single
title: Current Blog Page
---
{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{post.date | date: "%Y-%d-%m"}}</p>
<p>{{post.excerpt }}</p>
{% endfor %}
