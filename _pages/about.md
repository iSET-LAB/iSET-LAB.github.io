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

/* --- IMAGE FLOATS RIGHT (WRAPPED BY 2ND PARAGRAPH) --- */
.image {
    float: right; /* Moves the image to the right */
    margin-left: 20px; /* Space between image and text */
    margin-bottom: 10px; /* Space below the image */
    width: 30%; /* Adjust size as needed */
}

.image img {
    width: 100%;
    max-width: 300px; /* Reduce the image size for better wrapping */
    border-radius: 5px;
    display: block;
}

/* --- PARAGRAPH STYLES --- */
.full-width {
    clear: both; /* Ensures full-width paragraphs are separate */
    width: 100%;
    display: block;
}

.wrap-text {
    overflow: hidden; /* Prevents text overlap */
    text-align: justify; /* Clean text wrap */
}

/* --- RESPONSIVE LAYOUT FOR SMALL SCREENS --- */
@media (max-width: 768px) {
    .image {
        float: none; /* Removes float on small screens */
        width: 100%; /* Image takes full width */
        margin-left: 0;
        text-align: center;
    }
    
    .wrap-text {
        text-align: left; /* Align text normally on small screens */
    }
}
</style>

<div class="container">
    <h1>Welcome to iSET Lab</h1>
    
    <!-- First paragraph (full width) -->
    <p class="full-width">
        The iSET Lab's commitment is to explore intelligent systems and emerging technologies that shape the future of various industries (e.g., civil engineering and construction) while encompassing the diverse research areas it covers.
    </p>

    <!-- Second paragraph (wraps around the image) -->
    <div class="wrap-text">
        <div class="image">
            <img src="/_pages/lab_group_pictire.jpg" alt="Lab Members Group Picture">
        </div>
        <p>
            To pursue the long-term interdisciplinary research vision of future workforce development and digital twin towards a more sustainable and resilient civil/construction industry, iSET Lab will focus on multidisciplinary solutions informed by data science, AI (ML/DL/GenAI), HPC, BIM, human factors engineering, drone technology, wearable devices, signal processing, and VR/AR.
        </p>
    </div>

    <!-- Third paragraph (full width) -->
    <p class="full-width">
        The director of iSET Lab, Dr. Md Nazmus Sakib, is an Assistant Professor of Construction Engineering and Management in the Department of Civil Engineering and the Department of Computer Science and Engineering (affiliated) at The University of Texas at Arlington.
    </p>
</div>


## News
### Latest Updates from iSET Lab

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

