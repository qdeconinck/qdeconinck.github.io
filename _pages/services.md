---
title: "Services"
layout: textlay
excerpt: "Quentin De Coninck's Services."
sitemap: false
permalink: /services/
---

# Services

## Conference Organization

<ul>
{% for service in site.data.servlist %}
{% if service.type == "conf_org" %}
<li> {{ service.name }} </li>
{% endif %}
{% endfor %}
</ul>

## Technical Program Committee Participation

<ul>
{% for service in site.data.servlist %}
{% if service.type == "tpc" %}
<li> {{ service.name }} </li>
{% endif %}
{% endfor %}
</ul>

## Other Reviewing Activities

### Journal

<ul>
{% for service in site.data.servlist %}
{% if service.type == "ext_jour" %}
<li> {{ service.name }} </li>
{% endif %}
{% endfor %}
</ul>

### Conference (external reviews)

<ul>
{% for service in site.data.servlist %}
{% if service.type == "ext_conf" %}
<li> {{ service.name }} </li>
{% endif %}
{% endfor %}
</ul>
