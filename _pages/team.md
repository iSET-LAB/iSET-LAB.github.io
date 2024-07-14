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