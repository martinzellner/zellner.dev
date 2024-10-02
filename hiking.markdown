---
title: Hiking
layout: page
---

# {{ page.title }}

Find my hiking adventures here:

{% for post in site.posts %}
{% if post.path contains 'hiking' %}
 * [{{ post.title }}]({{ post.url }}) on {{ post.date | date: "%Y-%m-%d" }}


{% endif %}
{% endfor %}