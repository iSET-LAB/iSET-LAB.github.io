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
        border-radius: 50%;
        margin: 10px;
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
