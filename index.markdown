---
layout: default
title: Oykun Yilmaz, Designer.
image: /assets/oykun.jpg
---
<div class="max-width">
	{% for post in site.posts %}
		<article>
			<h1 class="slim"><a href="{{ post.url }}" title="Read more">{{ post.title }}</a></h1>
			<time datetime="{{ post.date | date: '%B %-d, %Y' }}" class="text-grey text-small">{{ post.date | date: "%B %-d, %Y" }}</time>
		</article>
	{% endfor %}
</div>