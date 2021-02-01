---
layout: default
title: Oykun Yilmaz, Designer.
---

<div class="col-12">

{% for post in site.posts %}
<div class="row">
	<article>
		<h1 class="slim"><a href="{{ post.url }}">{{ post.title }}</a></h1>
		<time datetime="{{ post.date | date: '%B %-d, %Y' }}" class="text-grey text-small">{{ post.date | date: "%B %-d, %Y" }}</time>
	</article>
</div>
{% endfor %}

</div>