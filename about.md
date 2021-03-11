---
layout: page
title: This page is all about me
---

## Project

{{ site.description }}

## Team

{% for team_member in site.team_members %}
- **Name:** {{ team_member.name }}, **Role**: {{ team_member.role }}
 
{% endfor %}


## Alumni

{% for alumnus in site.alumni %}
- **Name:** {{ alumnus.name }}
 
{% endfor %}
