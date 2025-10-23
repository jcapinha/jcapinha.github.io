---
layout: default
title: About Me
---

<!-- Fixed Image on Right -->
<div class="about-fixed-image">
    <div class="image-container">
        <img src="{{ site.data.about.hero.image.src }}" alt="{{ site.data.about.hero.image.alt }}">
    </div>
</div>

<!-- Scrollable Content Area -->
<div class="about-scrollable-content">
    
    <!-- Hero Introduction Section -->
    <div class="about-hero">
        <h1>{{ site.data.about.hero.title }}</h1>
        <h2 class="hero-tagline">{{ site.data.about.hero.tagline }}</h2>
        <p class="hero-description">{{ site.data.about.hero.content }}</p>
    </div>

    <!-- Story Sections -->
    <div class="story-sections">
    
    <!-- The Journey Section -->
    <div class="story-section journey-section">
        <div class="section-header">
            <h2>{{ site.data.about.journey.title }}</h2>
            <h3>{{ site.data.about.journey.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.journey.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.journey.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    <!-- Curiosity & Deep Dives Section -->
    <div class="story-section curiosity-section">
        <div class="section-header">
            <h2>{{ site.data.about.curiosity.title }}</h2>
            <h3>{{ site.data.about.curiosity.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.curiosity.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.curiosity.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    <!-- Seeking New Horizons Section -->
    <div class="story-section new-horizons-section">
        <div class="section-header">
            <h2>{{ site.data.about.new_horizons.title }}</h2>
            <h3>{{ site.data.about.new_horizons.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.new_horizons.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.new_horizons.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    <!-- Leadership & Mentorship Section -->
    <div class="story-section leadership-section">
        <div class="section-header">
            <h2>{{ site.data.about.leadership.title }}</h2>
            <h3>{{ site.data.about.leadership.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.leadership.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.leadership.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
            {% if site.data.about.leadership.blog_reference %}
            <div class="blog-reference">
                <p><em>{{ site.data.about.leadership.blog_reference }}</em></p>
            </div>
            {% endif %}
        </div>
    </div>

    <!-- Communication as a Superpower Section -->
    <div class="story-section communication-section">
        <div class="section-header">
            <h2>{{ site.data.about.communication.title }}</h2>
            <h3>{{ site.data.about.communication.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.communication.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.communication.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    <!-- Values & Impact Section -->
    <div class="story-section values-section">
        <div class="section-header">
            <h2>{{ site.data.about.values.title }}</h2>
            <h3>{{ site.data.about.values.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.values.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.values.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    <!-- Hobbies & Life Outside Work Section -->
    <div class="story-section hobbies-section">
        <div class="section-header">
            <h2>{{ site.data.about.hobbies.title }}</h2>
            <h3>{{ site.data.about.hobbies.subtitle }}</h3>
        </div>
        <div class="section-content">
            <p>{{ site.data.about.hobbies.content }}</p>
            <ul class="highlights">
                {% for highlight in site.data.about.hobbies.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>
        </div>
    </div>

    </div>
    
</div>