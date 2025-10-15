---
layout: default
title: Home
---

<div class="hero-section">
    <h1>Hello, I'm João Capinha</h1>
    <p class="tagline">Bridging the gap between product vision and technical excellence</p>
</div>

<div class="intro-section">
    <p class="lead">
        As a Product Owner with a deep technical background, I transform complex data challenges into user-centric solutions. Currently based in Paris, I bring 6+ years of experience in steering data platforms and backend systems from concept to reality.
    </p>
    
    <div class="highlights">
        <div class="highlight-item">
            <h3>💡 Vision & Strategy</h3>
            <p>Translating business needs into actionable technical roadmaps and leading teams to deliver impactful solutions.</p>
        </div>
        <div class="highlight-item">
            <h3>🚀 Innovation & Scale</h3>
            <p>Proven track record of modernizing legacy systems and scaling data platforms on AWS, boosting team velocity by 40%.</p>
        </div>
        <div class="highlight-item">
            <h3>🤝 Leadership</h3>
            <p>Passionate about fostering collaboration between stakeholders and empowering teams to achieve their best work.</p>
        </div>
    </div>
</div>

<div class="explore-section">
    <h2>Explore More</h2>
    <div class="explore-grid">
        <a href="/about" class="explore-card">
            <h3>👋 About Me</h3>
            <p>Get to know me beyond the professional realm – my journey, interests, and what drives me in both technology and life.</p>
            <span class="explore-link">Learn more about me →</span>
        </a>
        
        <a href="/cv" class="explore-card">
            <h3>💼 My Experience</h3>
            <p>Dive into my professional background at BMW Group, including key achievements in product ownership and data engineering.</p>
            <span class="explore-link">View full CV →</span>
        </a>
        
        <a href="/blog" class="explore-card">
            <h3>✍️ Blog & Insights</h3>
            <p>Read my thoughts on product management, data engineering, and technology trends through articles and case studies.</p>
            <span class="explore-link">Browse articles →</span>
        </a>
    </div>
</div>

<style>
.hero-section {
    text-align: left;
    margin: 2em 0 3em;
}

.hero-section h1 {
    font-size: 3em;
    margin-bottom: 0.2em;
    color: #0E4E45;
}

.tagline {
    font-size: 1.4em;
    color: #666;
    margin-bottom: 2em;
}

.intro-section {
    max-width: 900px;
}

.lead {
    font-size: 1.2em;
    line-height: 1.6;
    margin-bottom: 2em;
    color: #2C3E50;
}

.highlights {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2em;
    margin-top: 3em;
}

.highlight-item {
    padding: 1.5em;
    background: white;
    border-radius: 10px;
    box-shadow: 0 4px 20px rgba(14, 78, 69, 0.08);
    transition: transform 0.2s ease;
}

.highlight-item:hover {
    transform: translateY(-5px);
}

.highlight-item h3 {
    color: #0E4E45;
    margin-top: 0;
    margin-bottom: 0.8em;
}

.highlight-item p {
    color: #2C3E50;
    margin: 0;
    line-height: 1.5;
}

.explore-section {
    margin-top: 4em;
    padding-top: 2em;
    border-top: 1px solid rgba(14, 78, 69, 0.1);
}

.explore-section h2 {
    color: #0E4E45;
    margin-bottom: 1.5em;
}

.explore-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2em;
}

.explore-card {
    padding: 2em;
    background: white;
    border-radius: 12px;
    box-shadow: 0 4px 20px rgba(14, 78, 69, 0.08);
    text-decoration: none;
    transition: all 0.3s ease;
    border: 1px solid rgba(14, 78, 69, 0.1);
}

.explore-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 25px rgba(14, 78, 69, 0.12);
    border-color: #0E4E45;
}

.explore-card h3 {
    color: #0E4E45;
    margin: 0 0 0.8em 0;
    font-size: 1.3em;
}

.explore-card p {
    color: #2C3E50;
    margin: 0 0 1.5em 0;
    line-height: 1.6;
}

.explore-link {
    color: #0E4E45;
    font-weight: 500;
    display: inline-block;
}

.explore-card:hover .explore-link {
    text-decoration: underline;
}

@media (max-width: 768px) {
    .hero-section h1 {
        font-size: 2.5em;
    }
    
    .tagline {
        font-size: 1.2em;
    }
    
    .highlights {
        grid-template-columns: 1fr;
    }
    
    .explore-grid {
        grid-template-columns: 1fr;
    }
    
    .explore-card {
        padding: 1.5em;
    }
}
</style>