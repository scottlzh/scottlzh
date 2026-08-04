---
layout: page
title: projects
permalink: /projects/
description: Funded projects and sponsored research in the Transportation Intelligence Lab.
nav: true
nav_order: 3
horizontal: true
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>

<h2>Funding Agencies and Research Support</h2>

<div class="row row-cols-1 row-cols-md-2">
  <div class="col mb-4">
    <div class="card h-100">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: center;">
        <img src="{{ '/assets/img/logo/FHWA.png' | relative_url }}" alt="Federal Highway Administration logo" style="width: 96px; max-height: 72px; object-fit: contain;">
        <div>
          <strong>Federal Highway Administration (FHWA)</strong><br>
          Exploratory Advanced Research Program support for pedestrian video analytics.
        </div>
      </div>
    </div>
  </div>
  <div class="col mb-4">
    <div class="card h-100">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: center;">
        <img src="{{ '/assets/img/logo/USDOT.png' | relative_url }}" alt="U.S. Department of Transportation logo" style="width: 96px; max-height: 72px; object-fit: contain;">
        <div>
          <strong>U.S. Department of Transportation (USDOT)</strong><br>
          Support through safety, freight, and university transportation center programs.
        </div>
      </div>
    </div>
  </div>
  <div class="col mb-4">
    <div class="card h-100">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: center;">
        <img src="{{ '/assets/img/logo/FERSC.png' | relative_url }}" alt="FERSC University Transportation Center logo" style="width: 96px; max-height: 72px; object-fit: contain;">
        <div>
          <strong>University Transportation Center for Freight Transportation for Efficient and Resilient Supply Chain (FERSC)</strong><br>
          Research support for freight resilience, extreme-weather logistics, and rural delivery systems.
        </div>
      </div>
    </div>
  </div>
  <div class="col mb-4">
    <div class="card h-100">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: center;">
        <img src="{{ '/assets/img/logo/MarTREC.png' | relative_url }}" alt="Maritime Transportation Research and Education Center logo" style="width: 96px; max-height: 72px; object-fit: contain;">
        <div>
          <strong>Maritime Transportation Research and Education Center (MarTREC)</strong><br>
          Support for port recovery and maritime transportation resilience research.
        </div>
      </div>
    </div>
  </div>
  <div class="col mb-4">
    <div class="card h-100">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: center;">
        <img src="{{ '/assets/img/logo/TAMU_Engineering.png' | relative_url }}" alt="Texas A&M Engineering logo" style="width: 96px; max-height: 72px; object-fit: contain;">
        <div>
          <strong>Texas A&amp;M Engineering</strong><br>
          Dissertation research support for cyber-physical resilience of connected and automated vehicle systems.
        </div>
      </div>
    </div>
  </div>
</div>
