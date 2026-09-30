---
layout: page
permalink: /people/maria-montez-rath/
title: Maria Montez Rath
person: maria-montez-rath
nav: false
---

{%- assign p = site.data.people | where: "slug", page.person | first -%}

<style>
.profile { display: flex; gap: 2rem; flex-wrap: wrap; align-items: flex-start; }
.profile img { width: 220px; max-width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 8px; }
.profile .info { flex: 1; min-width: 260px; }
.profile h2 { margin-top: 0; }
.profile .role { color: var(--global-text-color-light); font-style: italic; margin: 0; }
.profile .links { margin: .8rem 0; }
.profile .links a { margin-right: 1rem; }
.profile .tags { list-style: none; padding: 0; display: flex; flex-wrap: wrap; gap: .4rem; }
.profile .tags li { border: 1px solid var(--global-divider-color); border-radius: 999px; padding: .1rem .7rem; font-size: .85rem; }
</style>

<div class="profile">
<img src="{{ '/assets/img/people/' | append: p.photo | relative_url }}" alt="{{ p.name }}">
<div class="info">
<h2>{{ p.name }}</h2>
{%- for t in p.titles -%}<p class="role">{{ t }}</p>{%- endfor -%}
<p class="links"><a href="mailto:{{ p.email }}">✉ {{ p.email }}</a>{%- if p.profile_url -%}<a href="{{ p.profile_url }}">Stanford Profile</a>{%- endif -%}{%- if p.scholar_url -%}<a href="{{ p.scholar_url }}">Google Scholar</a>{%- endif -%}</p>
<h4>About</h4>
<p>{%- if p.bio -%}{{ p.bio }}{%- else -%}Bio coming soon.{%- endif -%}</p>
<h4>Expertise</h4>
<ul class="tags">{%- for e in p.expertise -%}<li>{{ e }}</li>{%- endfor -%}</ul>
</div>
</div>

<p style="margin-top:2rem"><a href="{{ '/people/' | relative_url }}">&larr; Back to all people</a> · <a href="{{ '/publications/' | relative_url }}">Core publications</a></p>
