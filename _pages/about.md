---
permalink: /
title: false
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* --- STYLES FOR THE FLEX LAYOUT (WELCOME TEXT & IMAGE) --- */
<style>
/* --- FLEX LAYOUT WITH WRAPPING --- */
.container {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: flex-start;
    gap: 20px;
}

.text {
    flex: 2;
    min-width: 300px; /* Ensures text has a minimum width before wrapping */
}

.image {
    flex: 1;
    text-align: center;
    order: -1; /* Moves the image to the left when there's space */
}

.image img {
    width: 100%;
    max-width: 500px;
    border-radius: 5px;
}

/* --- RESPONSIVENESS: SWITCH TO COLUMN LAYOUT ON SMALL SCREENS --- */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
  .image {
    order: 0; /* Reset order so image appears above/below text on small screens */
  }
}
</style>

<div class="container">
  <div class="image">
    <!-- Update the image path as needed for your site structure -->
    <img src="/_pages/lab_group_pictire.jpg" alt="Lab Members Group Picture">
  </div>
  <div class="text">
    <h1>Welcome to iSET Lab</h1>
    <p>
      The iSET Lab's commitment is to explore intelligent systems and emerging technologies that shape the future of various industries (e.g., civil engineering and construction) while encompassing the diverse research areas it covers.
    </p>
    <p>
      To pursue the long-term interdisciplinary research vision of future workforce development and digital twin towards a more sustainable and resilient civil/construction industry, iSET Lab will focus on multidisciplinary solutions informed by data science, AI (ML/DL/GenAI), HPC, BIM, human factors engineering, drone technology, wearable devices, signal processing, and VR/AR.
    </p>
    <p>
      The director of iSET Lab, Dr. Md Nazmus Sakib, is an Assistant Professor of Construction Engineering and Management in the Department of Civil Engineering and the Department of Computer Science and Engineering (affiliated) at The University of Texas at Arlington.
    </p>
  </div>
</div>

---

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

