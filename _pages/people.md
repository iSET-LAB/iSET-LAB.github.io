---
permalink: /People/
title: "Principal Investigator"
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---

# Lab Members

{% for member in site.data.people %}
## {{ member.name }}

![Profile Image]({{ member.image }})

**Position:** {{ member.position }}

**Research Interests:** {{ member.research_interests }}

**Email:** [{{ member.email }}](mailto:{{ member.email }})

[LinkedIn]({{ member.linkedin }}) | [Google Scholar]({{ member.google_scholar }}) | [CV]({{ member.cv }})

---
{% endfor %}