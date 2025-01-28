---
permalink: /hudai/
title: false
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

<style>
    .publication {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
    }

    .publication img {
        max-width: 150px; /* Adjust the size as needed */
        height: auto;
        margin-right: 20px;
    }

    .publication-info {
        max-width: 800px; /* Adjust the max width as needed */
    }

    .publication-info a {
        font-size: 1.2em;
        color: #007BFF;
        text-decoration: none;
    }

    .publication-info p {
        margin-top: 5px;
    }
</style>

# Publications

Welcome to our Publications page! Here you'll find a collection of our lab's publications.

{% for publication in site.data.publications %}
<div class="publication">
    <img src="{{ '/images/' | append: publication.image | relative_url }}" alt="{{ publication.title }}">
    <div class="publication-info">
        <a href="{{ publication.link }}" target="_blank">{{ publication.title }}</a>
        <p>{{ publication.description }}</p>
    </div>
</div>
{% endfor %}