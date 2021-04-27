---
layout: default
title: Oykun Yilmaz, Designer.
tagline: Oykun's personal website and blog on design, development and lessons learned in life.   
description: Oykun's personal website and blog on design, development and lessons learned in life.   
image: /assets/social_image.jpg
---
<div>
	{% for post in site.posts %}
        <div class="separator">
            <article class="max-width flex justify-between items-center">
                <div class="w-60 pr3">
                    <h1 class="slim"><a href="{{ post.url }}" title="Read more"> {{ post.title }} </a></h1>
                    <time datetime="{{ post.date | date: '%B %-d, %Y' }}" class="text-grey text-small">{{ post.date | date: "%B %-d, %Y" }}</time>
                </div>
                <div class="w-40 tc">
                    <a href="{{ post.url }}" title="Read more"><img src="{{ post.image }}" height="250"></a>
                </div>
            </article>
        </div>
	{% endfor %}
</div>