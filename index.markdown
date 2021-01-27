---
layout: default
title: Oykun Yilmaz, Designer.
---

{% for post in site.posts %}
  <article>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}" class="text-grey">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %}