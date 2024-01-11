---
title: Home
layout: home
nav_order: 1
---

# Robot Operating Systems
{: .no_toc }
ROB 320, Winter 2024 at the University of Michigan
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Meeting Times
**Lecture** - Monday, Wednesday - 10:30-12:00 - 1050 FRB

**Lab** - Friday - 2:30-4:30 - 1050 FRB

# Instructor

<div class="staff-row">
{% assign instructors = site.staff | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}
</div>

{% assign gsis = site.staff | where: 'role', 'Graduate Student Instructor' %}
{% assign num_gsis = gsis | size %}
{% if num_gsis != 0 %}

# Graduate Instructor

<div class="staff-row">
{% assign gsis = site.staff | where: 'role', 'Graduate Student Instructor' %}
{% for staffer in gsis %}
{{ staffer }}
{% endfor %}
</div>
{% endif %}

{% assign teaching_assistants = site.staff | where: 'role', 'Instructional Aide' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

# Instructional Aides

<div class="staff-row">
{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
</div>
{% endif %}

{% assign development_staff = site.staff | where: 'role', 'Development Staff' %}
{% assign num_development_staff = development_staff | size %}
{% if num_development_staff != 0 %}

# Development Staff

<div class="staff-row">
{% for staffer in development_staff %}
{{ staffer }}
{% endfor %}
</div>
{% endif %}

# Office Hours
*coming soon*
