---
layout: page
title: Garden
category: published
order: 2
---

{% for post in site.posts %}
  <li><a style="{% if page.url == post.url %}color:#db8b97;{% endif %}" href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}