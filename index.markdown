---
layout: default
title: "Oykun Yilmaz, Designer."
tagline: "Personal website and blog on design, development and lessons learned in life."
description: "Personal website and blog on design, development and lessons learned in life."  
image: /assets/social_image.jpg
bgcolor: ffffff
---
<div class="w-100-l flex justify-between flex-wrap">
    <div class="w-70-l">
        {% for post in site.posts %}
            <div class="separator">
                <article class="max-width flex-l justify-between flex-wrap items-center">
                    <div class="w-70-l">
                        <h1 class="slim"><a href="{{ post.url }}" title="Read more"> {{ post.title }} </a></h1>
                    </div>
                    <div class="w-20-l tr-l">
                        <time datetime="{{ post.date | date: '%B %-d, %Y' }}" class="text-grey text-small">{{ post.date | date: "%b %-d, %Y" }}</time>
                        <!-- <a href="{{ post.url }}" title="Read more"><img src="{{ post.image }}"></a> -->
                    </div>
                </article>
            </div>
        {% endfor %}
    </div>
    <div class="w-20-l">
        {% include sidebar.html %}
    </div>
</div>