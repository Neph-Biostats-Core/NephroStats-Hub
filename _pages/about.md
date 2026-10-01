---
layout: about
title: about
permalink: /
subtitle:

selected_papers: true # shows papers marked `selected={true}` in _bibliography/papers.bib
social: false

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
---

{%- assign L = site.data.links -%}

<style>
/* hide the default name header on the home page; the banner replaces it */
.post-header { display: none; }
.hero { background: #8C1515; color: #fff; border-radius: 12px; padding: 2.75rem 2.5rem; margin: 0 0 2rem; display: flex; align-items: center; justify-content: space-between; gap: 2rem; flex-wrap: wrap; }
.hero .text { flex: 1 1 380px; }
.hero .eyebrow { text-transform: uppercase; letter-spacing: .12em; font-size: .8rem; opacity: .85; margin: 0 0 .5rem; }
.hero h1 { color: #fff; font-size: 2.3rem; line-height: 1.15; margin: 0 0 .75rem; font-weight: 600; }
.hero p.lead { color: #fff; opacity: .92; font-size: 1.05rem; margin: 0 0 1.5rem; max-width: 34rem; }
.hero .logo { flex: 0 1 300px; text-align: center; }
.hero .logo img { width: 100%; max-width: 300px; filter: brightness(0) invert(1); }
.btn-hero { display: inline-block; padding: .65rem 1.25rem; border-radius: 6px; font-weight: 600; text-decoration: none !important; margin: 0 .6rem .6rem 0; transition: transform .15s, box-shadow .15s; }
.btn-hero:hover { transform: translateY(-2px); box-shadow: 0 4px 12px rgba(0,0,0,.25); }
.btn-hero.primary { background: #fff; color: #8C1515 !important; }
.btn-hero.ghost { border: 2px solid #fff; color: #fff !important; }
.stats { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; margin: 0 0 2.25rem; text-align: center; }
.stats .stat { border: 1px solid var(--global-divider-color); border-radius: 10px; padding: 1rem .5rem; }
.stats .num { font-size: 1.9rem; font-weight: 700; color: #8C1515; line-height: 1.1; }
.stats .label { font-size: .85rem; color: var(--global-text-color-light); }
.services { display: grid; grid-template-columns: repeat(auto-fit, minmax(230px, 1fr)); gap: 1.25rem; margin: 0 0 2.5rem; }
.service { border: 1px solid var(--global-divider-color); border-top: 4px solid #8C1515; border-radius: 10px; padding: 1.4rem 1.3rem; display: flex; flex-direction: column; }
.service .icon { font-size: 1.6rem; color: #8C1515; margin-bottom: .6rem; }
.service h3 { font-size: 1.15rem; margin: 0 0 .5rem; }
.service p { font-size: .93rem; margin: 0 0 .9rem; flex: 1; }
.service a.more { font-weight: 600; font-size: .92rem; }
.section-title { font-size: 1.5rem; margin: 0 0 1rem; }
@media (max-width: 576px) { .hero { padding: 2rem 1.4rem; } .hero h1 { font-size: 1.8rem; } .stats { grid-template-columns: 1fr; } }
</style>

<section class="hero">
<div class="text">
<p class="eyebrow">Division of Nephrology · Stanford Medicine</p>
<h1>Stanford Nephrology Biostatistics Core</h1>
<p class="lead">We partner with faculty and fellows of the Division of Nephrology on the design, conduct, analysis and publication of kidney-related research.</p>
<a class="btn-hero primary" href="{{ L.support_request_form }}">Request Support</a><a class="btn-hero ghost" href="{{ L.office_hours_signup }}">Sign up for Office Hours</a>
</div>
<div class="logo"><img src="{{ '/assets/img/biostats-logo.png' | relative_url }}" alt="Stanford Medicine · Biostatistics Core, Division of Nephrology"></div>
</section>

<div class="stats">
<div class="stat"><div class="num">{{ site.data.people.size }}</div><div class="label">biostatisticians &amp; analysts</div></div>
<div class="stat"><div class="num">180+</div><div class="label">publications &amp; presentations since 2020</div></div>
<div class="stat"><div class="num">2×</div><div class="label">office hours every month</div></div>
</div>

<h2 class="section-title">How we can help</h2>
<div class="services">
<div class="service">
<div class="icon"><i class="fa-solid fa-file-signature"></i></div>
<h3>Project &amp; Grant Support</h3>
<p>Study design, sample size, analysis plans, grant statistical sections and manuscript support, matched to a statistician with the right expertise.</p>
<a class="more" href="{{ L.support_request_form }}">Submit a request &rarr;</a>
<a class="more" href="{{ L.protocol_template }}">Protocol template &rarr;</a>
</div>
<div class="service">
<div class="icon"><i class="fa-solid fa-calendar-check"></i></div>
<h3>Office Hours</h3>
<p>Twice a month for quick questions. Two statisticians, one Master's and one Doctorate level, are available at each session.</p>
<a class="more" href="{{ L.office_hours_signup }}">Sign up for a Zoom link &rarr;</a>
</div>
<div class="service">
<div class="icon"><i class="fa-solid fa-people-group"></i></div>
<h3>KCR Conference</h3>
<p>Monday Kidney Clinical Research sessions: didactic lectures, research presentations, methods and grant discussions.</p>
<a class="more" href="{{ L.kcr_schedule }}">Full schedule &rarr;</a>
<a class="more" href="{{ L.kcr_signup }}">Sign up to present &rarr;</a>
</div>
</div>

<p>Meet the <a href="{{ '/people/' | relative_url }}">team</a>, browse our <a href="{{ '/publications/' | relative_url }}">publications</a>, or find <a href="{{ '/resources/' | relative_url }}">resources</a>.</p>
