---
title: "Research"
permalink: /projects/
---

## Selected Projects
Below are selected projects written in an artifact-first format: objective, approach, and outputs.

{% assign items = site.projects | sort: "date" | reverse %}
{% for p in items %}
### [{{ p.title }}]({{ p.url }})
**One-line summary:** {{ p.summary }}

- **Objective:** {{ p.objective }}
- **Approach:** {{ p.approach }}
- **Outputs:** {{ p.outputs }}

{% if p.links %}
- **Links:**
  {% for l in p.links %}
  - {{ l.label }}: {{ l.url }}
  {% endfor %}
{% endif %}

---
{% endfor %}
