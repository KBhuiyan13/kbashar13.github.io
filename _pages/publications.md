---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}


# ⭐ Selected Publications

{% assign selected = site.publications | where: "selected", true %}

{% for post in selected %}
  {% include archive-single.html %}
{% endfor %}

---

# 📖 Journal Articles

{% assign journals = site.publications | where: "type", "Journal" %}

{% for post in journals %}
  {% include archive-single.html %}
{% endfor %}

---

# 🎤 Conference Papers

{% assign conferences = site.publications | where: "type", "Conference" %}

{% for post in conferences %}
  {% include archive-single.html %}
{% endfor %}

---

# 📚 Book Chapters

{% assign books = site.publications | where: "type", "Book Chapter" %}

{% for post in books %}
  {% include archive-single.html %}
{% endfor %}

---

# 📄 Preprints

{% assign preprints = site.publications | where: "type", "Preprint" %}

{% for post in preprints %}
  {% include archive-single.html %}
{% endfor %}

# 📝 Under Review

{% assign review = site.publications | where: "status", "Under Review" %}

{% for post in review %}
  {% include archive-single.html %}
{% endfor %}



