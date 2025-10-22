---
layout: default
title: Home
---

<div class="hero-section">
    <h1>{{ site.data.home.hero.title }}</h1>
    <p class="tagline">{{ site.data.home.hero.tagline }}</p>
</div>

<div class="intro-section">
    <p class="lead">{{ site.data.home.intro.lead }}</p>
    
    <div class="highlights">
        {% for highlight in site.data.home.highlights %}
        <div class="highlight-item">
            <h3>{{ highlight.icon }} {{ highlight.title }}</h3>
            <p>{{ highlight.description }}</p>
        </div>
        {% endfor %}
    </div>
</div>

<div class="explore-section">
    <h2>{{ site.data.home.explore.title }}</h2>
    <div class="explore-grid">
        {% for card in site.data.home.explore.cards %}
        <a href="{{ card.url }}" class="explore-card">
            <h3>{{ card.icon }} {{ card.title }}</h3>
            <p>{{ card.description }}</p>
            <span class="explore-link">{{ card.link_text }}</span>
        </a>
        {% endfor %}
    </div>
</div>
