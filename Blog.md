---
layout: page
title: "Blog"
permalink: /Blog
---

{% for post in site.posts %}
<hr>
<h2 style="margin-bottom: 20px;"><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.excerpt | strip_html | truncate: 150 }} <a href="{{ post.url }}">Read more</a></p>
{% endfor %}
