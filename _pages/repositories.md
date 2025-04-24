---
layout: page
permalink: /repositories/
title: repositories
# description: Edit the `_data/repositories.yml` and change the `github_users` and `github_repos` lists to include your own GitHub profile and repositories.
nav: true
nav_order: 4
---
<!-- 
{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %} -->

## 👨‍💻 Public GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

<br>
<br>
<br>

## 💻 Company GitHub Contributions

While many of my contributions are in private company repositories, I remain an active developer:

<p align="center">
  <img src="/assets/img/Screenshot from 2025-03-06 14-27-06.png" alt="49 contributions in the last year - Company GitHub Activity" />
</p>
> **49 contributions in the last year** to company projects, primarily focused on developing LLM-powered platforms and AI solutions. My work includes LangChain implementations, custom RAG solutions, and backend infrastructure development.