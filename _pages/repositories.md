---
layout: page
permalink: /repositories/
title: projects / repositories
description: Below are the most recent GitHub repositories I have worked on. The top four are part of my PhD project along with their publication links. 
nav: true
nav_order: 3
---


{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
