---
layout: page
permalink: /publications/
title: Publications
description: Peer-reviewed papers, preprints, and selected research outputs from the lab.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<style>
@media (max-width: 575.98px) {
  .publications .abbr {
    text-align: center;
  }

  .publications .abbr abbr.badge,
  .publications .abbr figure {
    max-width: 8rem;
    margin-left: auto;
    margin-right: auto;
  }

  .publications .abbr figure {
    margin-bottom: 1rem;
  }

  .publications .abbr img.preview {
    width: 100%;
    max-width: 8rem;
  }
}
</style>

<p><small>* Corresponding author.</small></p>

<div class="publications">

<h2>Top-tier AI Conference Papers</h2>

{% bibliography --query @inproceedings %}

<h2>Peer-Reviewed Journal Articles</h2>

{% bibliography --query @article %}

</div>
