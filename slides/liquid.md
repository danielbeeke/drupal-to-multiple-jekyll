
/app/_layouts/projects.html

```
---
layout: html
---
{% assign sorted_projects = 
    (site.data.projects | sort: 'created') %}

<div class="projects-overview">
    {% for project in sorted_projects %}
        {% include components/projects/teaser.html %}
    {% endfor %}
</div>
```