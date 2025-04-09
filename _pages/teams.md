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
        max-width: 250px;
        height: auto;
        margin: 10px;
        border-radius: 10px;
        box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
    }

    .align-center, .align-left, .align-right {
        display: flex;
        align-items: center;
        gap: 20px;
        margin-bottom: 20px;
    }

    .align-center {
        flex-direction: column;
        text-align: center;
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
        max-width: 500px;
        padding: 15px;
        text-align: justify;
    }

    .btn {
        padding: 8px 12px;
        margin: 5px;
        border-radius: 5px;
        text-decoration: none;
        font-size: 1.1em;
        transition: all 0.3s ease;
    }

    .btn-blue { color: #007BFF; }
    .btn-green { color: #28a745; }
    .btn-red { color: #dc3545; }
    
    .btn:hover {
        transform: scale(1.1);
    }
</style>

<!-- Centered heading and intro text -->
<h1 style="text-align: center;">Meet with our brilliant team members!</h1>
</p>

{% for member in site.data.team %}
<div class="align-{{ member.alignment }}">
    <img src="{{ '/images/' | append: member.image | relative_url }}" alt="{{ member.name }}" class="profile-pic">
    <div class="info">
        <h2>{{ member.name }}</h2>
        <p><strong>Position:</strong> {{ member.position }}</p>
        <p><strong>Description:</strong> {{ member.description }}</p>
        <p><strong>Research Interest:</strong> {{ member.research_interests }}</p>
        <p><strong>Email:</strong> <a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
        <p>
            <a href="{{ member.linkedin }}" class="btn btn-blue"><i class="fab fa-linkedin"></i></a>
            <a href="{{ member.google_scholar }}" class="btn btn-green"><i class="fas fa-graduation-cap"></i></a>
            <a href="{{ member.cv }}" class="btn btn-red"><i class="fas fa-file-alt"></i></a>
            <a href="{{ member.website }}" class="btn btn-red"><i class="fas fa-user"></i></a>
        </p>
    </div>
</div>
{% endif %}
{% endfor %}
