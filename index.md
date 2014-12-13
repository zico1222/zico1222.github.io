---
layout: default
title: 角煮の願い
description: Top page
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <h1><a href="{{ post.url }}">{{ post.title }}{% if post.tagline %}<small>{{post.tagline}}</small>{% endif %}</a></h1>
    <h6>{{ post.date | date_to_long_string }}</h6>
    {{ post.content }}
    <hr />
  {% endfor %}
</ul>
