---
permalink: /research/
title: "Research"
author_profile: true
---

## Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

{% if site.publications.size == 0 %}
Publications will appear here as they are added.
{% endif %}

---

## Working Papers

{% for post in site.publications reversed %}
  {% if post.status == "working paper" or post.status == "draft" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

---

## Research Projects

{% for project in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}

{% if site.portfolio.size == 0 %}
Research projects will appear here as they are added.
{% endif %}

