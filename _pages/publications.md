---
title: "Publications"
permalink: /publications/
---

## Papers & Preprints
Reverse-chronological list. Replace placeholders with your real entries.

{% assign items = site.publications | sort: "date" | reverse %}
{% for pub in items %}
### [{{ pub.title }}]({{ pub.url }})
{{ pub.authors }}  
**Venue/Status:** {{ pub.venue }} · **Year:** {{ pub.year }}

{% if pub.links %}
**Links:**
{% for l in pub.links %}
- {{ l.label }}: {{ l.url }}
{% endfor %}
{% endif %}

---
{% endfor %}
