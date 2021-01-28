---
layout: default
title: Oykun Yilmaz, Designer.
---

<div class="col-12">

{% for post in site.posts %}
<div class="row">
	<article>
		<a href="{{ post.url }}">{{ post.title }}</a>
		<time datetime="{{ post.date | date: "%Y-%m-%d" }}" class="text-grey text-small">{{ post.date | date_to_long_string }}</time>
	</article>
</div>
{% endfor %}

</div>