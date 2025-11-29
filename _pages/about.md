---
permalink: /
title: "Christian Fogel Henneberg"
author_profile: true
layout: splash
header:
  overlay_color: "#901a1e"
  overlay_filter: "0.5"
  cta_label: "Download CV"
  cta_url: "/cv/"
excerpt: "Third year PhD student in Economics at the University of Copenhagen. My research focuses on Economics of Education, with a particular emphasis on school choice, field experiments, and public policy."
# redirect_from removed - homepage is now separate from about page
---

## Christian Fogel Henneberg

I am a third year PhD student in Economics at the University of Copenhagen, enrolled in the 3+5 program. My research focuses on the study of public policies and regulation in education markets, with a particular emphasis on school choice, field experiments, and information barriers.

[Read more >](/about/) [Download CV](/cv/)

---

## Featured Research

{% for post in site.publications reversed limit:5 %}
  * **[{{ post.title }}]({{ post.url }})**  
    {% if post.venue %}{{ post.venue }}{% endif %}  
    {% if post.excerpt %}{{ post.excerpt | markdownify | strip_html | truncate: 160 }}{% endif %}
{% endfor %}

{% if site.publications.size == 0 %}
* Publications will appear here as they are added.
{% endif %}

[View all research >](/research/)

---

## Featured Projects

{% for project in site.portfolio limit:6 %}
  * **[{{ project.title }}]({{ project.url }})**  
    {% if project.excerpt %}{{ project.excerpt | markdownify | strip_html | truncate: 160 }}{% endif %}
{% endfor %}

{% if site.portfolio.size == 0 %}
* Projects will appear here as they are added.
{% endif %}

[View all projects >](/portfolio/)
