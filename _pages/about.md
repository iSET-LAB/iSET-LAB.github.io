---
permalink: /
title: false
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* --- CONTAINER STYLING --- */
.container {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
}

/* --- HEADER & NEWS TITLE STYLES WITH EFFECTS --- */
h1 {
    color: #0077cc; /* Blue color */
    font-size: 28px;
    font-weight: bold;
    text-shadow: 2px 2px 5px rgba(0, 119, 204, 0.3); /* Subtle glow effect */
    position: relative;
    display: inline-block;
    transition: all 0.3s ease-in-out;
}

h1:hover {
    color: #0055aa;
    text-shadow: 4px 4px 8px rgba(0, 119, 204, 0.5);
    transform: scale(1.05); /* Slight zoom effect */
}

/* --- LINE AFTER NEWS TITLE --- */
.news-title {
    color: #0077cc;
    font-size: 24px;
    font-weight: bold;
    position: relative;
}

.news-title::after {
    content: "";
    display: block;
    width: 100%;
    height: 2px;
    background-color: #0077cc;
    margin-top: 5px;
}

/* --- FLEX CONTAINER FOR IMAGE + TEXT --- */
.wrap-text {
    display: grid;
    grid-template-columns: 1fr auto; /* Text takes remaining space, image stays on the right */
    gap: 20px; /* Space between text and image */
    align-items: start;
    text-align: justify;
}

/* --- IMAGE STYLES --- */
.image {
    width: 30%; /* Keeps image proportionate */
}

.image img {
    width: 100%;
    height: auto;
    border-radius: 5px;
    display: block;
}

/* --- PARAGRAPH STYLES --- */
.full-width {
    clear: both;
    width: 100%;
    display: block;
    text-align: justify;
}

/* --- RESPONSIVE LAYOUT FOR SMALL SCREENS --- */
@media (max-width: 768px) {
    .wrap-text {
        grid-template-columns: 1fr; /* Stacks text and image on mobile */
        text-align: left;
    }

    .image {
        width: 100%;
        text-align: center;
    }
}
</style>

<div class="container">
    <h1>Welcome to iSET Lab</h1>
    
    <!-- First paragraph (full width) -->
    <div class="full-width">
        The iSET Lab's commitment is to explore intelligent systems and emerging technologies that shape the future of various industries (e.g., civil engineering and construction) while encompassing the diverse research areas it covers.
    </div>

    <!-- Second paragraph (wraps around the image, using grid layout) -->
    <div class="wrap-text">
        <div>
            To pursue the long-term interdisciplinary research vision of future workforce development and digital twin towards a more sustainable and resilient civil/construction industry, iSET Lab will focus on multidisciplinary solutions informed by data science, AI (ML/DL/GenAI), HPC, BIM, human factors engineering, drone technology, wearable devices, signal processing, and VR/AR.
        </div>
        <div class="image">
            <img src="/_pages/lab_group_pictire.jpg" alt="Lab Members Group Picture">
        </div>
    </div>

    <!-- Third paragraph (full width) -->
    <div class="full-width">
        The director of iSET Lab, Dr. Md Nazmus Sakib, is an Assistant Professor of Construction Engineering and Management in the Department of Civil Engineering and the Department of Computer Science and Engineering (affiliated) at The University of Texas at Arlington.
    </div>

    <!-- News Section -->
    <h2 class="news-title">Latest Updates from iSET Lab</h2>
    
    <div style="max-height: 200px; overflow-y: auto; border: 1px solid #ddd; padding: 15px; border-radius: 5px; background-color: #f9f9f9;">
      <ul style="margin: 0; padding-left: 1.5rem; list-style-type: disc;">
        <li>📢 <strong>[News Item 1]</strong> - Brief description of recent achievement, project, or event.</li>
        <li>📢 <strong>[News Item 2]</strong> - Another key update regarding the lab's work.</li>
        <li>📢 <strong>[News Item 3]</strong> - Highlighting a conference presentation, publication, or grant.</li>
        <li>📢 <strong>[News Item 4]</strong> - Another major development in the lab.</li>
        <li>📢 <strong>[News Item 5]</strong> - A new project collaboration or funding announcement.</li>
        <li>📢 <strong>[News Item 6]</strong> - Lab members receiving awards or recognitions.</li>
        <li>📢 <strong>[News Item 7]</strong> - Latest publications and research insights.</li>
      </ul>
    </div>

    <p>For more updates, stay connected with us!</p>
</div>
