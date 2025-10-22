---
layout: default
title: CV
permalink: /cv
---

<div class="cv-container">
    <div class="cv-sidebar">
        <div class="profile-section">
            <div class="profile-image">
                <img src="/assets/images/profile.jpg" alt="João Capinha">
            </div>
            <h1 class="name">{{ site.data.cv.personal_info.name }}</h1>
            <h2 class="title">{{ site.data.cv.personal_info.title }}</h2>
        </div>
        
        
        <div class="skills-section">
            <h3>Skills</h3>
            {% for skill_category in site.data.cv.skills %}
            <div class="skill-category">
                <h4>{{ skill_category[1].title }}</h4>
                <ul>
                    {% for item in skill_category[1].items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>
            {% endfor %}
        </div>
        
        <div class="languages-section">
            <h3>Languages</h3>
            {% for language in site.data.cv.languages %}
            <div class="language-item">
                <span class="language-name">{{ language.name }}</span>
                <div class="language-bar">
                    <div class="language-progress" style="width: {{ language.level }}%"></div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
    
    <div class="cv-main">
        <div class="summary-section">
            <h2>Summary</h2>
            <p>{{ site.data.cv.summary }}</p>
        </div>
        
        <div class="experience-section">
            <h2>Experience and Achievements</h2>
            {% for job in site.data.cv.experience %}
            <div class="job-item">
                <div class="job-header">
                    <h3>{{ job.position }}</h3>
                    <span class="company">{{ job.company }}</span>
                    <span class="period">{{ job.period }}</span>
                </div>
                <ul class="achievements">
                    {% for achievement in job.achievements %}
                    <li>{{ achievement }}</li>
                    {% endfor %}
                </ul>
            </div>
            {% endfor %}
        </div>
        
        <div class="education-section">
            <h2>Education</h2>
            {% for education in site.data.cv.education %}
            <div class="education-item">
                <h3>{{ education.degree }}</h3>
                <p class="institution">{{ education.institution }}</p>
                <span class="period">{{ education.period }}</span>
            </div>
            {% endfor %}
        </div>
        
        <div class="certifications-section">
            <h2>Certifications</h2>
            <div class="certifications-list">
                {% for cert in site.data.cv.certifications %}
                <span class="certification">{{ cert }}</span>
                {% endfor %}
            </div>
        </div>
    </div>
</div>
