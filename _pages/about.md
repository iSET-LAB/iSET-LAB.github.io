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
.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
}

.text {
    flex: 1;
    /* Optional: for visual spacing or design */
}

.image {
    flex: 1;
    text-align: center;
}

.image img {
    width: 50%;
    max-width: 500px;
    border-radius: 5px;
}

/* --- OPTIONAL: MOBILE RESPONSIVENESS --- */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>

<div class="container">
  <div class="text">
    <h1>Welcome to iSET Lab</h1>
    <p>
      The iSET Lab's commitment is to explore intelligent systems and emerging technologies that shape the future of various industries (e.g., civil engineering and construction) while encompassing the diverse research areas it covers.
    </p>
    <p>
      To pursue the long-term interdisciplinary research vision of future workforce development and digital twin towards a more sustainable and resilient civil/construction industry, iSET Lab will focus on multidisciplinary solutions informed by data science, AI (ML/DL), HPC, BIM, human factors engineering, drone technology, wearable devices, signal processing, and VR/AR.
    </p>
    <p>
      The director of iSET Lab, Dr. Md Nazmus Sakib, is an Assistant Professor of Construction Engineering and Management in the Department of Civil Engineering at The University of Texas at Arlington.
    </p>
  </div>
  <div class="image">
    <!-- Update the image path as needed for your site structure -->
    <img src="/_pages/lab_group_pictire.jpg" alt="Lab Members Group Picture">
  </div>
</div>

---

## News
### Latest Updates from iSET Lab

<!--
  Using pure HTML inside the scrollable div so it renders correctly.
  If you want more items, just add more <li> elements.
-->
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
