---
layout: archive
title: "Awards & Certifications"
permalink: /awards/
author_profile: true
---

# Awards

<div class="awards-grid">

{% for award in site.data.awards %}

<div class="award-card">

<h3>{{ award.icon }} {{ award.title }}</h3>

<p><strong>{{ award.organization }}</strong></p>

<p>{{ award.year }}</p>

<p>{{ award.description }}</p>

</div>

{% endfor %}

</div>

<hr>

# Certifications

<div class="awards-grid">

{% for cert in site.data.certifications %}

<div class="award-card">

<h3>{{ cert.icon }} {{ cert.title }}</h3>

<p><strong>{{ cert.issuer }}</strong></p>

<p>Issued: {{ cert.year }}</p>

<p><a href="{{ cert.credential }}" target="_blank">View Source</a></p>

</div>

{% endfor %}

</div>
