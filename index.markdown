---
layout: default
title: "Oykun Yilmaz, Designer."
tagline: "Personal website and blog on design, development and lessons learned in life."
description: "Personal website and blog on design, development and lessons learned in life."  
image: /assets/social_image.jpg
bgcolor: ffffff
---
<div>
	{% for post in site.posts %}
        <div class="separator">
            <article class="max-width flex-l justify-between flex-wrap items-center">
                <div class="w-60-l pr3">
                    <h1 class="slim"><a href="{{ post.url }}" title="Read more"> {{ post.title }} </a></h1>
                    <time datetime="{{ post.date | date: '%B %-d, %Y' }}" class="text-grey text-small">{{ post.date | date: "%B %-d, %Y" }}</time>
                </div>
                <div class="w-40-l tc">
                    <a href="{{ post.url }}" title="Read more"><img src="{{ post.image }}"></a>
                </div>
            </article>
        </div>
	{% endfor %}
</div>