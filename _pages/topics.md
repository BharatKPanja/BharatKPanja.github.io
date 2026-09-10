---
title: "Topics"
permalink: /topics/
author_profile: true
---

Longer-form pages on the areas I work in. This section grows over time — each new
topic is a file in the `_topics` folder.

{% for topic in site.topics %}
## [{{ topic.title }}]({{ topic.url | relative_url }})
{{ topic.excerpt | markdownify }}
{% endfor %}
