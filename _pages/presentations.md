---
permalink: /presentations/
title: "Presentations"
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

<style>
    .presentation {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
    }

    .presentation img {
        max-width: 150px; /* Adjust the size as needed */
        height: auto;
        margin-right: 20px;
    }

    .presentation-info {
        max-width: 800px; /* Adjust the max width as needed */
    }

    .presentation-info a {
        font-size: 1.2em;
        color: #007BFF;
        text-decoration: none;
    }

    .presentation-info p {
        margin-top: 5px;
    }
</style>

# Presentations

Welcome to our Presentations page! Here you'll find a collection of our lab's presentations.

{% for presentation in site.data.presentations %}
<div class="presentation">
    <img src="{{ '/images/' | append: presentation.image | relative_url }}" alt="{{ presentation.title }}">
    <div class="presentation-info">
        <a href="{{ presentation.link }}" target="_blank">{{ presentation.title }}</a>
        <p>{{ presentation.description }}</p>
    </div>
</div>
{% endfor %}
