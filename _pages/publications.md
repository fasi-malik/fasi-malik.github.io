---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

{% include bib_search.liquid %}

<!-- InspireHEP Citation Summary -->
{% assign inspire = site.data.inspirehep %}

<div class="card shadow-sm my-4 mx-auto" style="max-width: 420px;">
  <div class="card-body text-center">
    <h3 class="card-title mb-3">InspireHEP Citation Summary</h3>

    <div class="row">
      <div class="col-4">
        <p class="display-6 fw-bold text-primary mb-0">{{ inspire.papers }}</p>
        <p class="text-muted small">Papers</p>
      </div>
      <div class="col-4">
        <p class="display-6 fw-bold text-primary mb-0">{{ inspire.citations }}</p>
        <p class="text-muted small">Citations</p>
      </div>
      <div class="col-4">
        <p class="display-6 fw-bold text-primary mb-0">{{ inspire.hindex }}</p>
        <p class="text-muted small">h-index</p>
      </div>
    </div>

    <p class="mt-3 mb-0">
      <a href="https://inspirehep.net/authors/2047024" target="_blank">
        View on InspireHEP →
      </a>
    </p>
    <p class="text-muted small mb-0">Updated {{ inspire.updated }}</p>
  </div>
</div>

<!-- Publications List -->
<div class="publications">
{% bibliography --query @* --group_by year --sort_by month --order descending %}
</div>
