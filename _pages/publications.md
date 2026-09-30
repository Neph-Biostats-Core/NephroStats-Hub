---
layout: page
permalink: /publications/
title: publications
description: Papers and conference presentations by members of the Biostatistics Core (2020 onward), newest first. Core members' names are highlighted.
nav: true
nav_order: 2
---

<!-- _pages/publications.md
     Entries come from _bibliography/papers.bib. Each entry's `pubtype` field decides its section:
     paper = journal article, poster = poster / oral / published abstract, preprint = not yet peer reviewed, report = reports / software / proceedings. -->

<style>
.pub-section { font-size: 1.6rem; margin: 2.5rem 0 .5rem; padding-bottom: .35rem; border-bottom: 2px solid var(--global-theme-color); }
.pub-legend { font-size: .9rem; color: var(--global-text-color-light); }
</style>

{% include bib_search.liquid %}

<p class="pub-legend">Jump to: <a href="#papers">Journal articles</a> · <a href="#posters">Posters &amp; conference abstracts</a> · <a href="#preprints">Preprints</a> · <a href="#reports">Reports &amp; software</a></p>

<div class="publications">
<h2 class="pub-section" id="papers">Journal articles</h2>
{% bibliography --query @*[pubtype=paper]* %}
<h2 class="pub-section" id="posters">Posters &amp; conference abstracts</h2>
{% bibliography --query @*[pubtype=poster]* %}
<h2 class="pub-section" id="preprints">Preprints</h2>
{% bibliography --query @*[pubtype=preprint]* %}
<h2 class="pub-section" id="reports">Reports &amp; software</h2>
{% bibliography --query @*[pubtype=report]* %}
</div>
