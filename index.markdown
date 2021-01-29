---
layout: default
title: Oykun Yilmaz, Designer.
---

<div class="col-12">

{% for post in site.posts %}
<div class="row">
	<article>
		<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
		<time datetime="{{ post.date | date: "%Y-%m-%d" }}" class="text-grey text-small">{{ post.date | date_to_long_string }}</time>
	</article>
</div>
{% endfor %}

</div>