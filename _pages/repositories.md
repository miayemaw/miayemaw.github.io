---
layout: page
permalink: /talks/
title: talks
description: Invited talks, seminars, and workshops
nav: true
nav_order: 3
---

## Seminars & Invited Lectures

### 2025

**AI and Digital Twin for Smart Urban Air Mobility**  
*Invited Seminar, [Institution Name]*  
Date: [Month Year]

### 2024

**Deep Learning Applications in Aerospace Systems**  
*Invited Lecture, [Institution Name]*  
Date: [Month Year]

---

## Keynote Speeches

### 2023

**Future of Autonomous Aerial Vehicles**  
*Keynote Speaker, [Conference Name]*  
Date: [Month Year]

---

## Workshops

### 2023

**Reinforcement Learning for Mission Planning**  
*Workshop Instructor, [Event Name]*  
Date: [Month Year]

---

## Conference Presentations

Conference presentations are listed in the [Publications](/publications/) page.

## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  {% if site.data.repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %}

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
