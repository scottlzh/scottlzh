---
layout: page
title: projects
permalink: /projects/
description: Funded projects and sponsored research in the Transportation Intelligence Lab.
nav: true
nav_order: 3
horizontal: true
---

{% assign sorted_projects = site.projects | sort: "importance" %}

<!-- pages/projects.md -->
<div class="projects">
{% for project in sorted_projects %}
  {% include projects_horizontal.liquid %}
{% endfor %}
</div>

<h2>Additional Research Support</h2>

<div style="display: flex; flex-wrap: wrap; gap: 1rem; align-items: flex-start; padding: 1.1rem 0; border-bottom: 1px solid var(--global-divider-color);">
  <img src="{{ '/assets/img/logo/TAMU_Engineering.png' | relative_url }}" alt="Texas A&amp;M Engineering logo" style="width: 88px; max-height: 64px; object-fit: contain;">
  <div style="flex: 1 1 280px; min-width: 0;">
    <h3 style="font-size: 1.05rem; margin: 0 0 0.35rem;">Texas A&amp;M Engineering</h3>
    <div style="display: grid; grid-template-columns: 8.5rem minmax(0, 1fr); column-gap: 0.75rem; row-gap: 0.2rem; line-height: 1.5;">
      <strong>Program</strong>
      <span>Dissertation Fellowship</span>
      <strong>Role</strong>
      <span>Fellowship recipient</span>
      <strong>Content</strong>
      <span>Cyber-physical resilience of connected and automated vehicle systems.</span>
    </div>
  </div>
</div>
