---
layout: page
title: Projects
permalink: /projects/
---

<ul>
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
      {% if project.tags %}<small> — {{ project.tags | join: ", " }}</small>{% endif %}
      {% if project.summary %}<div>{{ project.summary }}</div>{% endif %}
    </li>
  {% endfor %}
</ul>
