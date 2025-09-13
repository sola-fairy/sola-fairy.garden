---
layout: page
title: Library
permalink: /library/
category: published
order: 1
---

<ul>
{% assign books_alpha = site.data.books | sort: "Title" %}
{% for book in books_alpha %}
    <li>{{ book.Title }}, {{ book.Genre }}</li>
{% endfor %}
</ul>

{% assign recommendations = site.data.books | where: 'Recommended', 'Yes' %}
{% for book in recommendations %}
    <img src="{{ book.CoverUrl }}" title="{{ book.Title }}" alt="Cover of {{ book.Title }}">
{% endfor %}
