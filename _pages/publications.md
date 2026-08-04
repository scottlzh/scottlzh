---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed papers, preprints, and selected research outputs from the lab.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<p><small>* Corresponding author.</small></p>

<div class="publications">

<h2>Peer-Reviewed Journal Articles</h2>

{% bibliography --query @article %}

<h2>Top-tier AI Conference Papers</h2>

{% bibliography --query @inproceedings %}

</div>
