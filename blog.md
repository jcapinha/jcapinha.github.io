---
layout: default
title: Blog
permalink: /blog
---

<div class="blog-timeline">
    {% for post in site.posts %}
    <article class="timeline-entry">
        <div class="timeline-content">
            <time class="date">{{ post.date | date: "%B %d, %Y" }}</time>
            <h2 class="title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
            <div class="excerpt">
                {{ post.excerpt }}
            </div>
            <a href="{{ post.url }}" class="read-more">Read More →</a>
        </div>
    </article>
    {% endfor %}
</div>

<style>
.blog-timeline {
    max-width: 800px;
    margin: 2em auto;
    position: relative;
}

.blog-timeline::before {
    content: '';
    position: absolute;
    left: -40px;
    top: 0;
    bottom: 0;
    width: 2px;
    background: #0E4E45;
}

.timeline-entry {
    position: relative;
    margin-bottom: 3em;
    padding-left: 1em;
}

.timeline-entry::before {
    content: '';
    position: absolute;
    left: -44px;
    top: 10px;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #0E4E45;
    border: 2px solid white;
}

.timeline-content {
    background: white;
    padding: 1.5em;
    border-radius: 8px;
    box-shadow: 0 2px 15px rgba(14, 78, 69, 0.1);
}

.date {
    display: block;
    color: #666;
    font-size: 0.9em;
    margin-bottom: 0.5em;
}

.title {
    margin: 0 0 0.5em;
    font-size: 1.6em;
}

.title a {
    color: #0E4E45;
    text-decoration: none;
}

.title a:hover {
    color: #156b5f;
}

.excerpt {
    color: #2C3E50;
    margin-bottom: 1em;
    line-height: 1.6;
}

.read-more {
    color: #0E4E45;
    text-decoration: none;
    font-weight: 500;
}

.read-more:hover {
    text-decoration: underline;
}
</style>
- Data Platforms
- Agile Leadership
- Cloud Technologies