---
layout: page
title: resources
permalink: /resources/
description: Forms, templates and learning materials. Internal resources require a Stanford (SUNet) login.
nav: true
nav_order: 5
---

<style>
.res-list { display: grid; gap: 1rem; margin-bottom: 2rem; }
.res-item { border: 1px solid var(--global-divider-color); border-left: 4px solid var(--global-theme-color); border-radius: 6px; padding: .9rem 1.1rem; }
.res-item.internal { border-left-color: #8C1515; }
.res-item h5 { margin: 0 0 .3rem; }
.res-item p { margin: 0; font-size: .95rem; }
.badge-login { display: inline-block; font-size: .72rem; font-weight: 600; background: #8C1515; color: #fff; border-radius: 3px; padding: .05rem .45rem; margin-left: .4rem; vertical-align: middle; }
</style>

## Public resources

Open to everyone.

<div class="res-list">
{%- for r in site.data.resources.public -%}
<div class="res-item"><h5><a href="{{ r.url }}">{{ r.name }}</a></h5><p>{{ r.description }}</p></div>
{%- endfor -%}
</div>

## Internal resources <span class="badge-login">🔒 Stanford login</span>

For Division of Nephrology faculty, fellows and staff. These links open Stanford-hosted content (Box, Smartsheet, SharePoint) that asks for your SUNet ID.

<div class="res-list">
{%- for r in site.data.resources.internal -%}
<div class="res-item internal"><h5><a href="{{ r.url }}">{{ r.name }}</a><span class="badge-login">🔒</span></h5><p>{{ r.description }}</p></div>
{%- endfor -%}
</div>

Missing something? Tell [Snow Yu](mailto:xueyu@stanford.edu) and we'll add it.
