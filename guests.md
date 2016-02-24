---
layout: page
title: Guests
---

{% for post in site.posts %}
{% if post.category == 'Guests' %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endif %}
{% endfor %}
