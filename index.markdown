---
layout: default
title: "Oykun Yilmaz, Designer."
tagline: "Personal website and blog on design, development and lessons learned in life."
description: "Personal website and blog on design, development and lessons learned in life."  
image: /assets/social_image.jpg
bgcolor: ffffff
---
<p class="mb5">Oykun is a <a href="https://crucial.design" target="_blank" title="Crucial Design Agencys">designer</a>, writer living in London, UK. <a href="/about" title="Oykun, About">Bio</a></p>

<h1>Writings</h1>
<ul class="square-list">
    {% for post in site.posts %}
    <li><a href="{{ post.url }}" title="Read more"> {{ post.title }} </a></li>
    {% endfor %}
</ul>