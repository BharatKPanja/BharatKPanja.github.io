---
title: "Projects"
permalink: /projects/
author_profile: true
---

Selected work and case studies — the migrations and platform programs behind the
résumé. Each project is a file in the `_projects` folder.

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url | relative_url }})
{{ project.excerpt | markdownify }}
{% endfor %}
