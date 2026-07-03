---
layout: archive
title: "People"
permalink: /people/
author_profile: true
css:
  - /assets/css/people.css
---

<h1>Research Advisors & Supervisors</h1>

<div class="people-grid">

{% for person in site.data.advisors %}

<div class="person-card">

  <img src="{{ person.photo | relative_url }}" class="person-photo" alt="{{ person.name }}">

  <h3>{{ person.name }}</h3>

  <p>
    <strong>{{ person.title }}</strong><br>
    {{ person.institution }}
  </p>

  <p>
    📧 <a href="mailto:{{ person.email }}">{{ person.email }}</a>
  </p>

  <p>
    <a href="{{ person.website }}" target="_blank">Website</a> ·
    <a href="{{ person.scholar }}" target="_blank">Google Scholar</a>
  </p>

  <p><strong>Role:</strong> {{ person.role }}</p>

  <p><strong>Research:</strong> {{ person.research }}</p>

  <p><em>{{ person.description }}</em></p>

</div>

{% endfor %}

</div>

<hr>

<h1>Research / Project Collaborators</h1>

<div class="collab-grid">

{% for person in site.data.collaborators %}

<div class="collab-card">

  <h3>{{ person.name }}</h3>

  <p><strong>{{ person.institution }}</strong></p>

  <p><em>{{ person.project }}</em></p>

  <p>{{ person.publication }}</p>

</div>

{% endfor %}

</div>
