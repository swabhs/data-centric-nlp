---
layout: home
title: CSCI 699. Data-Centric NLP
nav_exclude: true
permalink: index.html
seo:
  type: Course
  name: Data-Centric NLP
---

# {{ site.title }}
<!-- {: .mb-2 } {{ site.description }} {: .fs-6 .fw-300 } -->
{: .sp-2 }
USC Viterbi CSCI 699 &nbsp; 🍂 Fall 2022 &nbsp; ⏰ M/W 10:00 - 11:50am &nbsp; 📍 [WPH](https://maps.usc.edu/?id=1928&reference=THH#!m/552624?ct/53723,53722,55414,55415,55418) 203


<!-- ## Instructor -->
<!-- {:.no_toc} -->

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

<!-- ## Teaching Assistant -->
<!-- {:.no_toc} -->

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
{:.no_toc}

# Announcements

<!-- Announcements are stored in the `_announcements` directory and rendered according to the layout file, `_layouts/announcement.html`. -->

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
