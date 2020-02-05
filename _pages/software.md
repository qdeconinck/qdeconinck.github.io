---
title: "Quentin De Coninck - Software"
layout: textlay
excerpt: "Quentin De Coninck -- Software"
sitemap: false
permalink: /software/
---

# Software

As part of my applied research activities, I developed software.
They fall into three categories:

- **Prototypes** to demonstrate the feasibility of our solutions
- **Tools** to evaluate solutions
- **Data** such as network traces, databases,...

## Prototypes

<ul>
{% for soft in site.data.softlist %}

{% if soft.type == "prototype" %}
<li>
<pubtit>{{ soft.title }}</pubtit>
<p><em>{{ soft.authors }}</em></p>
<p>{{ soft.description }}</p>
{% for link in soft.links %}
<p><strong><a href="{{ link.url }}">{{ link.display }}</a></strong></p>
{% endfor %}
{% if soft.pubrelated %}
Related to the following publication(s): {{ soft.pubrelated }}
{% endif %}

</li>
{% endif %}
{% endfor %}
</ul>

## Tools

<ul>
{% for soft in site.data.softlist %}

{% if soft.type == "tools" %}
<li>
<pubtit>{{ soft.title }}</pubtit>
<p><em>{{ soft.authors }}</em></p>
<p>{{ soft.description }}</p>
{% for link in soft.links %}
<p><strong><a href="{{ link.url }}">{{ link.display }}</a></strong></p>
{% endfor %}
{% if soft.pubrelated %}
Related to the following publication(s): {{ soft.pubrelated }}
{% endif %}

</li>
{% endif %}
{% endfor %}
</ul>

## Data

<ul>
{% for soft in site.data.softlist %}

{% if soft.type == "data" %}
<li>
<pubtit>{{ soft.title }}</pubtit>
<p><em>{{ soft.authors }}</em></p>
<p>{{ soft.description }}</p>
{% for link in soft.links %}
<p><strong><a href="{{ link.url }}">{{ link.display }}</a></strong></p>
{% endfor %}
{% if soft.pubrelated %}
Related to the following publication(s): {{ soft.pubrelated }}
{% endif %}
</li>
{% endif %}
{% endfor %}
</ul>