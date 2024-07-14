---
permalink: /team/
title: "Team iSET"
author_profile: false
redirect_from: 
  - /md/
  - /markdown.html
---



{% for member in site.data.team %}
## {{ member.name }}

![Profile Image]({{ '/images/' | append: member.image | relative_url }})

**Position:** {{ member.position }}

**Research Interests:** {{ member.research_interests }}

**Email:** [{{ member.email }}](mailto:{{ member.email }})

[LinkedIn]({{ member.linkedin }}) | [Google Scholar]({{ member.google_scholar }}) | [CV]({{ member.cv }})

---
{% endfor %}