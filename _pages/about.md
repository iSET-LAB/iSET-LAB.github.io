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
    /*text-shadow: 2px 2px 5px rgba(0, 119, 204, 0.3); /* Subtle glow effect */*/
    position: relative;
    display: inline-block;
    transition: all 0.3s ease-in-out;
}

h1:hover {
    color: #0055aa;
    /*text-shadow: 4px 4px 8px rgba(0, 119, 204, 0.5);*/
    transform: scale(1.05); /* Slight zoom effect */
}

/* --- NEWS TITLE WITH UNDERLINE --- */
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
    display: flex;
    align-items: flex-start;
    gap: 20px; /* Space between text and image */
    text-align: justify;
}

/* --- IMAGE STYLES (DYNAMICALLY ADJUSTS TO TEXT HEIGHT) --- */
.image {
    flex: 0 0 250px; /* Keeps image width fixed */
    display: flex;
    align-items: stretch; /* Ensures image height matches text */
}

.image img {
    width: 100%;
    height: auto;
    border-radius: 5px;
    display: block;
}

/* --- PARAGRAPH STYLES --- */
.full-width {
    width: 100%;
    display: block;
    text-align: justify;
}

/* --- NEWS SECTION STYLES --- */
.news-container {
    max-height: 400px;     /* increased height */
    overflow-y: auto;      /* enable vertical scrolling when needed */
    border: 1px solid #ddd;
    padding: 12px;
    border-radius: 6px;
    background-color: #f9f9f9;
}

/* --- RESPONSIVE LAYOUT FOR SMALL SCREENS --- */
@media (max-width: 768px) {
    .wrap-text {
        flex-direction: column;
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

    <!-- Merged Second and Third Paragraph (wraps around image) -->
    <div class="wrap-text">
        <div>
            We believe that in today's world, the fields of science and technology are extremely broad to be defined by a single concentration. To pursue the long-term interdisciplinary research vision of future workforce development and digital twins towards a more sustainable and resilient Architecture, Engineering, and construction industry, iSET Lab will focus on multidisciplinary solutions informed by data science, AI (ML/DL/GenAI), HPC, BIM, human factors engineering, drone technology, wearable devices, signal processing, and XR (VR/AR/MR).
        </div>
        <div class="image">
            <img src="/_pages/lab_group_pictire.jpg" alt="Lab Members Group Picture">
        </div>
    </div>

    <!-- News Section -->
    <h2 class="news-title">Latest Updates from iSET Lab</h2>
    
    <div class="news-container">
      <ul style="margin: 0; padding-left: 1.5rem; list-style-type: disc;">
        <li>📢 <strong>August 21-2025</strong> - Dr. Sakib received a three-year $399,871 National Science Foundation IUSE grant for the project, <strong>Transforming Compliance Training for Drone Operators through an Extended Reality and Generative Artificial Intelligence-Driven System</strong>. This project will develop SKYGEN-XR, an advanced training system integrating XR and GenAI to enhance drone operation training for the AEC industry. <a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=2519021&HistoricalAwards=false" target="_blank">[NSF Award Details]</a></li>
        <li>📢 <strong>May 14-2025</strong> - iSET Lab presented 4 papers at the International Conference on Computing in Civil Engineering (i3CE 2025), New Orleans, May 11-14, 2025.</li>
        <li>📢 <strong>February 24-2025</strong> - Dr. Sakib got secondary affiliation with the Department of Computer Science at the University of Texas at Arlington.</li>
        <li>📢 <strong>January 24-2025</strong> - Abir Khan Ratul and Sanjay Acharjee joined the iSET Lab and the Department of Civil Engineering as the newest PhD students. They both completed B.Sc. in Civil Engineering from Bangladesh University of Engineering and Technology (BUET), Dhaka, Bangladesh.</li>
        <li>📢 <strong>January 24-2025</strong> - Dr. Sakib recognized by the Vice President for Student Affairs for contributions to the success Fall 2023 graduates at UTA.</li>
        <li>📢 <strong>August 23-2025</strong> - Dr. Sakib joined as Assistant Professor of Construction Engineering, Department of Civil Engineering at the University of Texas at Arlington.</li>
      </ul>
    </div>

    <p>For more updates, stay connected with us!</p>
</div>
