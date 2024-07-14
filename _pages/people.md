---
title: "People"
permalink: /people/
layout: single
---

# Lab Members

{% for member in site.data.people %}
## {{ member.name }}

![Profile Image]({{ member.image }})

**Position:** {{ member.position }}

**Research Interests:** {{ member.research_interests }}

**Email:** [{{ member.email }}](mailto:{{ member.email }})

---
{% endfor %}
