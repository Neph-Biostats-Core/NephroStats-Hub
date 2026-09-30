---
layout: page
title: people
permalink: /people/
description: Our team brings expertise in causal inference, survival analysis, trial design, large administrative data (USRDS, VA, claims, EHR) and statistical programming. Click a name to read more.
nav: true
nav_order: 1
---

<style>
.team-section { margin-top: 2rem; }
.team-section h2 { font-size: 1.5rem; border-bottom: 2px solid var(--global-theme-color); padding-bottom: .35rem; margin-bottom: 1.25rem; }
.team-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 1.75rem 1.5rem; }
.team-member { text-align: center; text-decoration: none !important; color: var(--global-text-color) !important; display: block; }
.team-member img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 50%; border: 3px solid var(--global-divider-color); transition: border-color .2s, transform .2s; }
.team-member:hover img { border-color: var(--global-theme-color); transform: translateY(-3px); }
.team-member .name { font-weight: 600; margin: .75rem 0 .15rem; color: var(--global-theme-color); }
.team-member .title { font-size: .85rem; color: var(--global-text-color-light); margin: 0; line-height: 1.35; }
</style>

{%- for g in site.data.people_groups -%}
{%- assign members = site.data.people | where: "group", g.id -%}
{%- if members.size > 0 -%}
<section class="team-section">
<h2>{{ g.title }}</h2>
<div class="team-grid">
{%- for p in members -%}
<a class="team-member" href="{{ '/people/' | append: p.slug | append: '/' | relative_url }}">
<img src="{{ '/assets/img/people/' | append: p.photo | relative_url }}" alt="{{ p.name }}" loading="lazy">
<p class="name">{{ p.name }}</p>
{%- for t in p.titles -%}<p class="title">{{ t }}</p>{%- endfor -%}
</a>
{%- endfor -%}
</div>
</section>
{%- endif -%}
{%- endfor -%}

<p style="margin-top:2.5rem">Not sure who to contact? <a href="{{ site.data.links.support_request_form }}">Submit a support request</a> and we'll route it.</p>
