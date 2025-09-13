---
layout: page
title: Library
permalink: /library/
category: published
order: 1
---

{% assign recommendations = site.data.books | where: 'Recommended', 'Yes' %}
{% for book in recommendations %}
    {% if book.Cover == nil %}
<h3>{{ book.Title }}</h3>
    {% else %}
<h3>{{ book.Title }}</h3><img src="{{ book.Cover }}" title="{{ book.Title }}" alt="Cover of {{ book.Title }}">
{% endif %}
{% endfor %}


