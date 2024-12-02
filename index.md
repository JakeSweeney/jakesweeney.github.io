---
layout: single
title: Home Page
---
## Latest Website Updates
<h2><a href="{{ site.posts.first.url }}">{{ site.posts.first.title }}</a></h2>
<p>{{site.posts.first.date | date: "%d-%m-%Y"}}</p>
<p>{{site.posts.first.excerpt }}</p>

## Pinned Items
[comment]: <>([About Me]({{ "/_posts/2024-12-02-AboutMe.md" | relative_url }})

{% for post in site.posts %}
{% if page.slug == AboutMe %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{post.date | date: "%d-%m-%Y"}}</p>
<p>{{post.excerpt }}</p>
{% endif %}
{% endfor %}