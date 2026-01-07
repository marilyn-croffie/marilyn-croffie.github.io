---
layout: page
title: Work
narrow: true
---

## Selected Projects

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url }})
**{{ project.context }}**  
{{ project.excerpt }}
{% endfor %}
