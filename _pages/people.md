---
layout: page
title: people
permalink: /people/
description: Our team brings expertise in causal inference, survival analysis, trial design, large administrative data (USRDS, VA, claims, EHR) and statistical programming.
nav: true
nav_order: 1
---

<style>
.people-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 1.5rem; margin-top: 1rem; }
.person-card { border: 1px solid var(--global-divider-color); border-radius: 8px; padding: 1rem; background: var(--global-bg-color); }
.person-card img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 6px; }
.person-card h5 { margin: .75rem 0 .25rem; }
.person-card .role { color: var(--global-text-color-light); font-style: italic; margin: 0; font-size: .9rem; }
.person-card .email { font-size: .85rem; margin: .3rem 0; word-break: break-all; }
.person-card .tags { list-style: none; padding: 0; margin: .5rem 0 0; display: flex; flex-wrap: wrap; gap: .3rem; }
.person-card .tags li { border: 1px solid var(--global-divider-color); border-radius: 999px; padding: 0 .55rem; font-size: .75rem; }
</style>

<div class="people-grid">
{%- for p in site.data.people -%}
<div class="person-card">
<img src="{{ '/assets/img/people/' | append: p.photo | relative_url }}" alt="{{ p.name }}" loading="lazy">
<h5>{{ p.name }}</h5>
{%- for t in p.titles -%}<p class="role">{{ t }}</p>{%- endfor -%}
<p class="email"><a href="mailto:{{ p.email }}">{{ p.email }}</a></p>
<ul class="tags">{%- for e in p.expertise -%}<li>{{ e }}</li>{%- endfor -%}</ul>
</div>
{%- endfor -%}
</div>

Not sure who to contact? [Submit a support request]({{ site.data.links.support_request_form }}) and we'll route it.
