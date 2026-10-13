---
layout: page
permalink: /people/gomathy-parvathinathan/
title: Gomathy Parvathinathan
person: gomathy-parvathinathan
nav: false
---

{%- assign p = site.data.people | where: "slug", page.person | first -%}

<style>
.person-page { display: grid; grid-template-columns: 240px 1fr; gap: 2.5rem; align-items: start; margin-top: .5rem; }
.person-page .photo img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; border-radius: 10px; box-shadow: 0 4px 14px rgba(0,0,0,.12); }
.person-page .roles { margin: 0 0 .9rem; }
.person-page .roles p { margin: 0; font-size: 1.05rem; color: var(--global-text-color-light); font-style: italic; }
.person-page .links { display: flex; flex-wrap: wrap; gap: .5rem; margin: 0 0 1.5rem; }
.person-page .links a { border: 1px solid var(--global-divider-color); border-radius: 999px; padding: .25rem .85rem; font-size: .9rem; text-decoration: none; }
.person-page .links a:hover { border-color: var(--global-theme-color); }
.person-page h4 { margin: 1.5rem 0 .6rem; font-size: 1.15rem; border-bottom: 2px solid var(--global-theme-color); padding-bottom: .3rem; }
.person-page h4:first-of-type { margin-top: 0; }
.person-page .bio p { line-height: 1.65; margin: 0 0 1rem; }
.person-page .tags { list-style: none; padding: 0; margin: 0; display: flex; flex-wrap: wrap; gap: .45rem; }
.person-page .tags li { border: 1px solid var(--global-divider-color); border-radius: 999px; padding: .15rem .75rem; font-size: .85rem; }
@media (max-width: 768px) { .person-page { grid-template-columns: 1fr; gap: 1.25rem; } .person-page .photo img { max-width: 220px; } }
</style>

<div class="person-page">
<div class="photo"><img src="{{ '/assets/img/people/' | append: p.photo | relative_url }}" alt="{{ p.name }}"></div>
<div class="info">
<div class="roles">{%- for t in p.titles -%}<p>{{ t }}</p>{%- endfor -%}</div>
<div class="links"><a href="mailto:{{ p.email }}">✉ {{ p.email }}</a>{%- if p.scholar_url -%}<a href="{{ p.scholar_url }}">Google Scholar</a>{%- endif -%}{%- if p.profile_url -%}<a href="{{ p.profile_url }}">Stanford Profile</a>{%- endif -%}</div>
<h4>About</h4>
<div class="bio">{%- if p.bio -%}{{ p.bio | markdownify }}{%- else -%}<p>Bio coming soon.</p>{%- endif -%}</div>
<h4>Expertise</h4>
<ul class="tags">{%- for e in p.expertise -%}<li>{{ e }}</li>{%- endfor -%}</ul>
</div>
</div>

<p style="margin-top:2.5rem"><a href="{{ '/people/' | relative_url }}">&larr; Back to all people</a> · <a href="{{ '/publications/' | relative_url }}">Core publications</a></p>
