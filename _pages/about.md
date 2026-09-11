---
layout: about
title: Home
permalink: /
subtitle: Reliable &middot; Resilient &middot; Intelligent &middot; Safe &middot; Efficient

lab_identity:
  logo: logo/lab/transportation-intelligence-lab-icon.png
  alt: R²ISE Transportation Lab logo

profile:
  align: right
  image: logo/lab/transportation-intelligence-lab-icon.png
  alt: R²ISE Transportation Lab visual identity
  image_circular: false # crops the image to make it circular
  home_visual: true

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  .home-link-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.65rem;
    margin: 1.1rem 0 1.35rem;
  }

  .home-link-row a {
    display: inline-flex;
    align-items: center;
    min-height: 2.15rem;
  }

  .lab-direction-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 0.85rem 0 1.4rem;
  }

  .lab-direction {
    border-top: 3px solid var(--global-theme-color);
    padding-top: 0.75rem;
  }

  .lab-direction strong {
    display: block;
    margin-bottom: 0.35rem;
    color: var(--global-text-color);
    font-size: 1rem;
    line-height: 1.35;
  }

  .lab-direction span {
    display: block;
    color: var(--global-text-color-light);
    line-height: 1.55;
  }

  .home-note {
    margin: 1rem 0 1.25rem;
    padding-left: 1rem;
    border-left: 3px solid var(--global-theme-color);
  }

  @media (max-width: 767.98px) {
    .lab-direction-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

The **R<sup>2</sup>ISE Transportation Lab** develops AI-enabled methods, models, and decision-support tools for transportation systems that are **reliable**, **resilient**, **intelligent**, **safe**, and **efficient**.

Led by Dr. Zihao (Scott) Li in the Department of Civil, Construction & Environmental Engineering at Marquette University, the lab works at the intersection of transportation engineering, multimodal AI, social-cyber-physical systems, traffic flow theory, connected and automated vehicles, freight systems, and infrastructure resilience.

<div class="home-link-row">
  <a class="btn btn-sm btn-outline-primary" href="{{ '/openings/' | relative_url }}">Openings</a>
  <a class="btn btn-sm btn-outline-primary" href="{{ '/projects/' | relative_url }}">Funded Projects</a>
  <a class="btn btn-sm btn-outline-primary" href="{{ '/publications/' | relative_url }}">Publications</a>
</div>

<div style="clear: both;"></div>

{% include figure.liquid loading="eager" path="assets/img/campus/marquette-panorama.jpg" class="img-fluid rounded z-depth-1" alt="Marquette University campus and Milwaukee transportation landscape" %}

## Research Directions

<div class="lab-direction-grid">
  <div class="lab-direction">
    <strong>AI for Transportation Intelligence</strong>
    <span>Multimodal and agentic AI, vision-language models, benchmark development, and knowledge-grounded decision support for transportation systems.</span>
  </div>
  <div class="lab-direction">
    <strong>Safety and Automation</strong>
    <span>Active traffic safety, vulnerable road user protection, connected and automated vehicle control, mixed autonomy traffic, and cyberattack-resilient operations.</span>
  </div>
  <div class="lab-direction">
    <strong>Resilience and Infrastructure Systems</strong>
    <span>Social-cyber-physical resilience, freight and port recovery, natural hazard disruption, traffic flow modeling, and infrastructure risk analysis.</span>
  </div>
</div>

<div class="home-note">
Prospective Ph.D. students, visiting students, and collaborators with overlapping interests are encouraged to review the openings, funded projects, and publications pages.
</div>
