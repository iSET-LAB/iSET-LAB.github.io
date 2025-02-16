---
permalink: /team/
title: false
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

<style>
    .profile-pic {
        max-width: 250px;  /* Adjust the max width as needed */
        height: auto;      /* Maintain the natural aspect ratio */
        margin: 10px;
    }

    .align-center {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        margin-bottom: 20px;
    }

    .align-left, .align-right {
        display: flex;
        align-items: flex-start;
        margin-bottom: 20px;
    }

    .align-left {
        flex-direction: row;
        text-align: left;
    }

    .align-right {
        flex-direction: row-reverse;
        text-align: right;
    }

    .info {
        padding: 0 15px;
        max-width: 500px; /* Adjust the max width as needed */
    }

    .btn {
        padding: 5px 10px;
        margin: 5px;
        border: none;
        color: white;
        text-decoration: none;
        font-size: 1.2em;
    }

    .btn-blue {
        color: #007BFF;
    }

    .btn-green {
        color: #28a745;
    }

    .btn-red {
        color: #dc3545;
    }
</style>

# Our Team

Welcome to the Team iSET page! Here you'll find information about our brilliant team members.

<div class="align-center">
    <img src="{{ '/images/MdNazmus_Sakib.jpg' | relative_url }}" alt="MD NAZMUS SAKIB" class="profile-pic">
    <div class="info">
        <h2>MD NAZMUS SAKIB, PH.D., A.M.ASCE, M.IEEE</h2>
        <p><strong>Position:</strong> Director</p>
        <p><strong>Research Interests:</strong> Artificial Intelligence, Data Science</p>
        <p><strong>Email:</strong> <a href="mailto:john.doe@university.edu">john.doe@university.edu</a></p>
        <p>
            <a href="https://linkedin.com/in/johndoe" class="btn btn-blue"><i class="fab fa-linkedin"></i></a>
            <a href="https://scholar.google.com/citations?user=johndoe" class="btn btn-green"><i class="fas fa-graduation-cap"></i></a>
            <a href="/files/john_doe_cv.pdf" class="btn btn-red"><i class="fas fa-file-alt"></i></a>
        </p>
    </div>
</div>

{% for member in site.data.team %}
{% if member.name != "MD NAZMUS SAKIB, PH.D., A.M.ASCE, M.IEEE" %}
<div class="align-{{ member.alignment }}">
    <img src="{{ '/images/' | append: member.image | relative_url }}" alt="{{ member.name }}" class="profile-pic">
    <div class="info">
        <h2>{{ member.name }}</h2>
        <p>{{ member.description }}</p>
        <p><strong>Email:</strong> <a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
        <p>
            <a href="{{ member.linkedin }}" class="btn btn-blue"><i class="fab fa-linkedin"></i></a>
            <a href="{{ member.google_scholar }}" class="btn btn-green"><i class="fas fa-graduation-cap"></i></a>
            <a href="{{ member.cv }}" class="btn btn-red"><i class="fas fa-file-alt"></i></a>
        </p>
    </div>
</div>
{% endif %}
{% endfor %}
