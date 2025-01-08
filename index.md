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
**Lecture**: Monday/Wednesday 10:30-12:00 in 1050 FRB

**Lab**: Friday 2:30-4:30 in 1050 FRB

# Instructor and Project Lead

<div class="staff-row">
{% assign instructors = site.staff | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}
</div>

{% assign devs = site.staff | where: 'role', 'Lead Developer' %}
{% assign num_devs = devs | size %}
{% if num_devs != 0 %}
# Lead Developer
<div class="staff-row">
{% assign devs = site.staff | where: 'role', 'Lead Developer' %}
{% for staffer in devs %}
{{ staffer }}
{% endfor %}
</div>
{% endif %}

{% assign gsis = site.staff | where: 'role', 'Graduate Student Instructor' %}
{% assign num_gsis = gsis | size %}
{% if num_gsis != 0 %}
# Graduate Student Instructor
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

[Office Hours Queue](https://oh.eecs.umich.edu/courses/rob320)
<br>
<iframe src="https://calendar.google.com/calendar/embed?src=c_41016a3477456b89a7e3e704284dc8d9bc54416ce78f5e1b61b7d7034f54cdae%40group.calendar.google.com&ctz=America%2FNew_York" style="border: 0" width="1400" height="600" frameborder="0" scrolling="no"></iframe>
