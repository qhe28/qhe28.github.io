---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

<!-- {% include bib_search.liquid %} -->

Systems composed of many interacting parts often exhibit dramatically different properties from their components:

> "There's no love in a carbon atom, no hurricane in a water molecule, [and] no financial collapse in a dollar bill."

I study how complex, emergent phenomena arise from simple microscopic rules within the framework of equilibrium statistical mechanics.
Specifically, I use probabilistic and combinatorial methods to rigorously characterize the Gibbs measures of various idealized physical systems across different temperatures, densities, and other parameters.

{% capture bib_count %}{% bibliography_count %}{% endcapture %}

<style>
  .publications {
    counter-reset: publication-counter {{ bib_count | plus: 1 }} !important;
  }
</style>

<div class="publications">

{% bibliography %}

</div>
