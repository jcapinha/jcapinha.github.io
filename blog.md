---
layout: default
title: Blog
permalink: /blog
---

<div class="blog-timeline">
    {% for post in site.posts %}
    <article class="blog-post">
        <div class="post-meta">{{ post.date | date: "%B %d, %Y" }}</div>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <div class="excerpt">
            {{ post.excerpt }}
        </div>
        <a href="{{ post.url }}" class="read-more">Read More</a>
    </article>
    {% endfor %}
</div>