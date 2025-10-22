---
layout: default
title: Contacts
---

<div class="contacts-container">
    <div class="contacts-header">
        <h1>Get In Touch</h1>
        <p>I'm always interested in discussing new opportunities, innovative projects, or just having a conversation about product management and data engineering.</p>
    </div>
    
    <div class="contacts-grid">
        <div class="contact-card">
            <div class="contact-icon">📍</div>
            <div class="contact-info">
                <h3>Location</h3>
                <p>{{ site.data.cv.personal_info.location }}</p>
            </div>
        </div>
        
        <div class="contact-card">
            <div class="contact-icon">📞</div>
            <div class="contact-info">
                <h3>Phone</h3>
                <p>{{ site.data.cv.personal_info.phone }}</p>
            </div>
        </div>
        
        <div class="contact-card">
            <div class="contact-icon">✉️</div>
            <div class="contact-info">
                <h3>Email</h3>
                <p><a href="mailto:{{ site.data.cv.personal_info.email }}">{{ site.data.cv.personal_info.email }}</a></p>
            </div>
        </div>
        
        <div class="contact-card">
            <div class="contact-icon">💼</div>
            <div class="contact-info">
                <h3>LinkedIn</h3>
                <p><a href="{{ site.data.cv.personal_info.linkedin_url }}" target="_blank" rel="noopener noreferrer">Connect with me on LinkedIn</a></p>
            </div>
        </div>
    </div>
    
    <div class="contacts-footer">
        <p>Feel free to reach out through any of these channels. I typically respond within 24 hours.</p>
    </div>
</div>
