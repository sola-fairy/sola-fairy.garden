---
layout: "post"
title: "Welcome to the Blog"
---

<h2>pages</h2>

{% for page in site.pages %}
  {% if page.category == "published" %}
<li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endif %}
{% endfor %}

<h2>posts</h2>

{% for post in site.posts %}
{{ post.title }} <br>
{% endfor %}