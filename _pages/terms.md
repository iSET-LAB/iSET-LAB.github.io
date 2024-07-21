---
permalink: /team/
title: "Team iSET"
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

<style>
    .profile-pic {
        max-width: 200px;  /* Adjust the max width as needed */
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
        align-items: center;
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

{% for member in site.data.team %}
<div class="align-{{ member.alignment }}">
    <img src="{{ '/images/' | append: member.image | relative_url }}" alt="{{ member.name }}" class="profile-pic">
    <div class="info">
        <h2>{{ member.name }}</h2>
        <p><strong>Position:</strong> {{ member.position }}</p>
        <p><strong>Research Interests:</strong> {{ member.research_interests }}</p>
        <p><strong>Email:</strong> <a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
        <p>
            <a href="{{ member.linkedin }}" class="btn btn-blue"><i class="fab fa-linkedin"></i></a>
            <a href="{{ member.google_scholar }}" class="btn btn-green"><i class="fas fa-graduation-cap"></i></a>
            <a href="{{ member.cv }}" class="btn btn-red"><i class="fas fa-file-alt"></i></a>
        </p>
    </div>
</div>
{% endfor %}
