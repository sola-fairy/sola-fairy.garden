---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Home
category: published
order: 1
---


{% for doc in site.docs %}
  {% if doc.category == "published" %}
  {{ doc.title }} <br>
  {% endif %}
{% endfor %}