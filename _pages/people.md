---
layout: page
title: people
permalink: /people/
nav: true
nav_order: 1
# Group photo: upload it as assets/img/group-photo.jpg (it appears automatically once uploaded)
group_photo: /assets/img/group-photo.jpg
group_photo_caption: The Stanford Nephrology Biostatistics Core team
---

<style>
.group-photo { margin: 0 0 2.5rem; }
.group-photo img { width: 100%; border-radius: 8px; display: block; }
.group-photo figcaption { text-align: center; font-size: .9rem; color: var(--global-text-color-light); margin-top: .5rem; }
.director { display: flex; gap: 1.75rem; align-items: flex-start; flex-wrap: wrap; background: var(--global-code-bg-color, rgba(0,0,0,.03)); border-left: 4px solid var(--global-theme-color); border-radius: 6px; padding: 1.5rem; margin-bottom: 2.5rem; }
.director img { width: 150px; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 50%; }
.director .msg { flex: 1; min-width: 260px; }
.director h2 { margin-top: 0; font-size: 1.5rem; }
.director .sig { margin-top: 1rem; font-weight: 600; }
.director .sig span { display: block; font-weight: 400; font-style: italic; color: var(--global-text-color-light); }
.team-section { margin-top: 2rem; }
.team-section h2 { font-size: 1.5rem; border-bottom: 2px solid var(--global-theme-color); padding-bottom: .35rem; margin-bottom: 1.25rem; }
.team-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 1.75rem 1.5rem; }
.team-member { text-align: center; text-decoration: none !important; color: var(--global-text-color) !important; display: block; }
.team-member img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 50%; border: 3px solid var(--global-divider-color); transition: border-color .2s, transform .2s; }
.team-member:hover img { border-color: var(--global-theme-color); transform: translateY(-3px); }
.team-member .name { font-weight: 600; margin: .75rem 0 .15rem; color: var(--global-theme-color); }
.team-member .title { font-size: .85rem; color: var(--global-text-color-light); margin: 0; line-height: 1.35; }
</style>

{%- assign gp = site.static_files | where: "path", page.group_photo | first -%}
{%- if gp -%}
<figure class="group-photo">
<img src="{{ page.group_photo | relative_url }}" alt="{{ page.group_photo_caption }}">
<figcaption>{{ page.group_photo_caption }}</figcaption>
</figure>
{%- endif -%}

{%- assign dm = site.data.director_message -%}
{%- if dm.message -%}
{%- assign d = site.data.people | where: "slug", dm.person | first -%}
<section class="director">
<img src="{{ '/assets/img/people/' | append: d.photo | relative_url }}" alt="{{ d.name }}">
<div class="msg">
<h2>Message from the Director</h2>
{{ dm.message | markdownify }}
<p class="sig">{{ d.name }}{%- for t in d.titles -%}<span>{{ t }}</span>{%- endfor -%}</p>
</div>
</section>
{%- endif -%}

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
