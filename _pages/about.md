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
.hero { position: relative; overflow: hidden; background: linear-gradient(135deg, #9b1c1c 0%, #8C1515 45%, #6a0f0f 100%); color: #fff; border-radius: 14px; padding: 3rem 2.75rem; margin: 0 0 2rem; display: flex; align-items: center; justify-content: space-between; gap: 2.5rem; flex-wrap: wrap; box-shadow: 0 10px 30px rgba(140,21,21,.25); }
.hero::before, .hero::after { content: ""; position: absolute; border-radius: 50%; pointer-events: none; }
.hero::before { width: 420px; height: 420px; right: -120px; top: -160px; background: radial-gradient(circle, rgba(255,255,255,.10) 0%, rgba(255,255,255,0) 70%); }
.hero::after { width: 260px; height: 260px; left: -90px; bottom: -130px; border: 1px solid rgba(255,255,255,.12); }
.hero > * { position: relative; z-index: 1; }
.hero .text { flex: 1 1 100%; max-width: 40rem; }
.hero .eyebrow { display: inline-block; text-transform: uppercase; letter-spacing: .14em; font-size: .72rem; font-weight: 600; color: rgba(255,255,255,.9) !important; background: rgba(255,255,255,.12); border: 1px solid rgba(255,255,255,.25); border-radius: 999px; padding: .3rem .8rem; margin: 0 0 1rem; }
.hero h1 { color: #fff !important; font-size: 2.4rem; line-height: 1.12; margin: 0 0 .9rem; font-weight: 700; letter-spacing: -.01em; }
.hero p.lead { color: rgba(255,255,255,.9) !important; font-size: 1.05rem; line-height: 1.55; margin: 0 0 1.75rem; max-width: 33rem; }
.brand-bar { margin: .25rem 0 1.25rem; }
.brand-bar img { height: 64px; width: auto; max-width: 100%; display: block; }
html[data-theme="dark"] .brand-bar img { filter: brightness(0) invert(1); opacity: .9; }
.btn-hero { display: inline-block; padding: .7rem 1.35rem; border-radius: 8px; font-weight: 600; font-size: .95rem; text-decoration: none !important; margin: 0 .6rem .6rem 0; transition: transform .15s, box-shadow .15s, background .15s; }
.btn-hero:hover { transform: translateY(-2px); box-shadow: 0 6px 16px rgba(0,0,0,.25); }
.btn-hero.primary { background: #fff; color: #8C1515 !important; }
.btn-hero.ghost { border: 1.5px solid rgba(255,255,255,.85); color: #fff !important; }
.btn-hero.ghost:hover { background: rgba(255,255,255,.12); }
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
@media (max-width: 768px) { .hero { padding: 2.25rem 1.5rem; } .hero h1 { font-size: 1.85rem; } .brand-bar img { height: 48px; } }
@media (max-width: 576px) { .stats { grid-template-columns: 1fr; } }
</style>

<div class="brand-bar"><img src="{{ '/assets/img/biostats-logo.png' | relative_url }}" alt="Stanford Medicine · Biostatistics Core, Division of Nephrology"></div>

<section class="hero">
<div class="text">
<p class="eyebrow">Statistical collaboration for kidney research</p>
<h1>Stanford Nephrology Biostatistics Core</h1>
<p class="lead">We partner with faculty and fellows of the Division of Nephrology on the design, conduct, analysis and publication of kidney-related research.</p>
<a class="btn-hero primary" href="{{ L.support_request_form }}">Request Support</a><a class="btn-hero ghost" href="{{ L.office_hours_signup }}">Sign up for Office Hours</a>
</div>
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
