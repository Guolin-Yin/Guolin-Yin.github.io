---
layout: page
permalink: /repositories/
title: Code
description: Repositories for my papers and other useful research tools
nav: true
nav_order: 7
---

{% if site.data.repositories.github_users %}

## My GitHub

<div class="repositories d-flex flex-wrap flex-md-row flex-column align-items-stretch">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid user=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column align-items-stretch">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %}

## My Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column align-items-stretch">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

## Useful Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column align-items-stretch">
  {% for repo in site.data.repositories.useful_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
