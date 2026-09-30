---
layout: page
title: resources
permalink: /resources/
description: Templates, forms and vetted learning materials.
nav: true
nav_order: 5
---

{% assign L = site.data.links %}

#### Templates & forms

- [Project/Grant Support Request Form]({{ L.support_request_form }})
- [Protocol Template]({{ L.protocol_template }})
- [Office hours sign-up]({{ L.office_hours_signup }})

#### Educational resources

{% for r in site.data.resources %}
**[{{ r.name }}]({{ r.url }})**
{{ r.description }}
{% endfor %}
