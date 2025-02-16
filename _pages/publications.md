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

## Conference Proceeding
{% assign conf_pubs = site.data.publications | where: "category", "Conference Proceeding" %}
{% for pub in conf_pubs %}
- {{ pub.reference }} 
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Journal Article
{% assign journal_pubs = site.data.publications | where: "category", "Journal Article" %}
{% for pub in journal_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}

## Other
{% assign other_pubs = site.data.publications | where: "category", "Other" %}
{% for pub in other_pubs %}
- {{ pub.reference }}
  {% if pub.link %}[Link]({{ pub.link }}){% endif %}
{% endfor %}
