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
    
    <div class="explore-grid">
        {% for card in site.data.home.explore.cards %}
        <a href="{{ card.url }}" class="explore-card">
            <span class="explore-link">{{ card.link_text }}</span>
            <p>{{ card.description }}</p>
        </a>
        {% endfor %}
    </div>
</div>
