---
layout: default
title: CV
permalink: /cv
---

<div class="cv-container">
    <!-- Sidebar with Profile and Skills -->
    <aside class="cv-sidebar">
        <!-- Profile Section -->
        <div class="profile-section">
            <div class="profile-image">
                <img src="{{ site.data.about.hero.image.src }}" alt="{{ site.data.cv.personal_info.name }}">
            </div>
            <h2 class="name">{{ site.data.cv.personal_info.name }}</h2>
            <p class="title">{{ site.data.cv.personal_info.title }}</p>
        </div>

        <!-- Contact Section -->
        <div class="contact-section">
            <h3>Contact</h3>
            <div class="contact-item">
                <strong>Location</strong>
                {{ site.data.cv.personal_info.location }}
            </div>
            <div class="contact-item">
                <strong>Phone</strong>
                {{ site.data.cv.personal_info.phone }}
            </div>
            <div class="contact-item">
                <strong>Email</strong>
                <a href="mailto:{{ site.data.cv.personal_info.email }}">{{ site.data.cv.personal_info.email }}</a>
            </div>
            <div class="contact-item">
                <strong>LinkedIn</strong>
                <a href="{{ site.data.cv.personal_info.linkedin_url }}" target="_blank">{{ site.data.cv.personal_info.linkedin }}</a>
            </div>
        </div>

        <!-- Languages Section -->
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

        <!-- Skills Section -->
        <div class="skills-section">
            <h3>Skills</h3>
            
            <div class="skill-category">
                <h4>{{ site.data.cv.skills.product_strategy.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.product_strategy.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.communication.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.communication.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.agile_scrum.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.agile_scrum.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.data_technologies.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.data_technologies.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.cloud_devops.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.cloud_devops.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.analytics_visualization.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.analytics_visualization.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.scaled_frameworks.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.scaled_frameworks.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>

            <div class="skill-category">
                <h4>{{ site.data.cv.skills.collaboration_tools.title }}</h4>
                <ul>
                    {% for item in site.data.cv.skills.collaboration_tools.items %}
                    <li>{{ item }}</li>
                    {% endfor %}
                </ul>
            </div>
        </div>
    </aside>

    <!-- Main Content Area -->
    <main class="cv-main">
        <!-- Summary Section -->
        <section class="summary-section">
            <h2>Summary</h2>
            <p>{{ site.data.cv.summary }}</p>
        </section>

        <!-- Experience Section -->
        <section class="experience-section">
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
        </section>

        <!-- Education Section -->
        <section class="education-section">
            <h2>Education</h2>
            {% for edu in site.data.cv.education %}
            <div class="education-item">
                <h3>{{ edu.degree }}</h3>
                <span class="institution">{{ edu.institution }}</span>
                <span class="period">{{ edu.period }}</span>
            </div>
            {% endfor %}
        </section>

        <!-- Certifications Section -->
        <section class="certifications-section">
            <h2>Certifications</h2>
            <div class="certifications-list">
                {% for cert in site.data.cv.certifications %}
                <span class="certification">{{ cert }}</span>
                {% endfor %}
            </div>
        </section>
    </main>
</div>
