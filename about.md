---
layout: page
title: This page is all about me
---

## Project

{{ site.description }}

## Team

{% for team_member in site.team_members | where_exp: "item", "item.role != 'alumni'" %}
- **Name:** {{ team_member.name }}, **Role**: {{ team_member.role }}
 
{% endfor %}
