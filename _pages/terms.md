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
        width: 150px;
        height: 150px;
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
    }

    .btn-blue {
        background-color: #007BFF;
    }

    .btn-green {
        background-color: #28a745;
    }

    .btn-red {
        background-color: #dc3545;
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
            <a href="https://linkedin.com/in/johndoe" class="btn btn-blue">LinkedIn</a>
            <a href="https://scholar.google.com/citations?user=johndoe" class="btn btn-green">Google Scholar</a>
            <a href="/files/john_doe_cv.pdf" class="btn btn-red">CV</a>
        </p>
    </div>
</div>

{% assign count = 0 %}
{% for member in site.data.team %}
<div class="{% if count | modulo: 2 == 0 %}align-left{% else %}align-right{% endif %}">
    <img src="{{ '/images/' | append: member.image | relative_url }}" alt="{{ member.name }}" class="profile-pic">
    <div class="info">
        <h2>{{ member.name }}</h2>
        <p><strong>Position:</strong> {{ member.position }}</p>
        <p><strong>Research Interests:</strong> {{ member.research_interests }}</p>
        <p><strong>Email:</strong> <a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
        <p>
            <a href="{{ member.linkedin }}" class="btn btn-blue">LinkedIn</a>
            <a href="{{ member.google_scholar }}" class="btn btn-green">Google Scholar</a>
            <a href="{{ member.cv }}" class="btn btn-red">CV</a>
        </p>
    </div>
</div>
{% assign count = count | plus: 1 %}
{% endfor %}
