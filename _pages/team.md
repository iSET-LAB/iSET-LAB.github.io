---
permalink: /Team/
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

<span style="margin-right: 10px;">
  [LinkedIn]({{ member.linkedin }}){: .btn .btn-blue}
</span>
<span style="margin-right: 10px;">
  [Google Scholar]({{ member.google_scholar }}){: .btn .btn-green}
</span>
<span>
  [CV]({{ member.cv }}){: .btn .btn-red}
</span>

---
{% endfor %}