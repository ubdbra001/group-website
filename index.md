---
layout: page
title: "Learning how to build websites with Jekyll"
---

## Description

{{ site.description }}

{% assign lead = site.team_members | where: "role", "project lead" | first %}  
The project is led by: {{ lead.name }}.  
See our full team [here](./about)

## Blogposts

{% for post in site.posts | sort: "date", "last" %}
- **{{ post.title }}** - {{ post.author }} ({{ post.date | date_to_string }})

{% endfor %}
