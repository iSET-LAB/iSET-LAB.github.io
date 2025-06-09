---
permalink: /publications/
title: false
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

# Publications

<!-- You can add an introductory paragraph if desired -->
<!-- <p>Welcome to our Publications page! Here you'll find a collection of our lab's publications.</p> -->

## Journal Article
{% assign journal_pubs = site.data.publications | where: "category", "Journal Article" %}
{% for pub in journal_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Conference Proceeding
{% assign conf_pubs = site.data.publications | where: "category", "Conference Proceeding" %}
{% for pub in conf_pubs %}
- {{ pub.reference }} 
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Dissertation & Thesis
{% assign other_pubs = site.data.publications | where: "category", "Dissertation & Thesis" %}
{% for pub in other_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Dataset
{% assign other_pubs = site.data.publications | where: "category", "Dataset" %}
{% for pub in other_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Presentation
{% assign other_pubs = site.data.publications | where: "category", "Presentation" %}
{% for pub in other_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Posters
{% assign poster_pubs = site.data.publications | where: "category", "Poster" %}
{% for pub in poster_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}
