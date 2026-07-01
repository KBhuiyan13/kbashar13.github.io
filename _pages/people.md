---
layout: archive
title: "People"
permalink: /people/
author_profile: true
---

# Research Advisors & Supervisors

<div class="people-grid">

{% for person in site.data.advisors %}

<div class="person-card">

<img src="{{ person.photo }}" class="person-photo">

## {{ person.name }}

**{{ person.title }}**

{{ person.institution }}

📧 {{ person.email }}

[Website]({{ person.website }})

[Google Scholar]({{ person.scholar }})

**Role:** {{ person.role }}

**Research:** {{ person.research }}

{{ person.description }}

</div>

{% endfor %}

</div>

---

# Research / Project Collaborators

<div class="collab-grid">

{% for person in site.data.collaborators %}

<div class="collab-card">

### {{ person.name }}

**{{ person.institution }}**

*{{ person.project }}*

{{ person.publication }}

</div>

{% endfor %}

</div>
