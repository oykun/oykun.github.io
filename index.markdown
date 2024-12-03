---
layout: default
title: "Oykun Yilmaz, Designer."
tagline: "Personal website and blog on design, development and lessons learned in life."
description: "Personal website and blog on design, development and lessons learned in life."  
image: /assets/social_image.jpg
bgcolor: ffffff
---
<h1>Oykun, Designer</h1>
<div class="flex mb5 mt1">
    <p class="ma0">I'm a <a href="https://crucial.design" target="_blank" title="Crucial Design Agencys">designer</a> and <a href="/books" title="Books and Articles">writer</a> with 25+ years of experience living in London. <a href="/bio" title="Oykun, About">Bio</a></p>
    <img src="/assets/oykun_avatar.jpg" alt="oykun" width="64" height="64" class="fr ml2">
</div>

<h1>Writings</h1>
<ul class="list ma0 pa0">
    {% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
    {% for year in posts_by_year %}
    <li><strong>{{ year.name }}</strong>
        <ul class="square-list ma0">
            {% for post in year.items %}
            <li><a href="{{ post.url }}" title="Read more"> {{ post.title }} </a></li>
            {% endfor %}
        </ul>
    </li>
    {% endfor %}
</ul>