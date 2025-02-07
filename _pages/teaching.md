---
title: "Quentin De Coninck - Teaching"
layout: textlay
excerpt: "Quentin De Coninck -- Teaching"
sitemap: false
permalink: /teaching/
---

# Teaching

My teaching contributions fall into two categories.
On the one hand, I am teaching cybersecurity-related courses at the University (UMONS, Belgium), serving both lectures and practical sessions.
On the other hand, I have contributions to several tutorials that have been presented during academic conferences.
In the past, I was involved in the organization of practical sessions at UCLouvain.

## University Courses

I teach the following courses.

<ul>

{% for course in site.data.courselist %}
<li>
<p><a href="{{ course.link }}">{{ course.title }}</a></p>
</li>

{% endfor %}

</ul>

## Tutorials

<ul>
{% for tuto in site.data.tutolist %}
<li>
<pubtit>{{ tuto.title }}</pubtit>
<p><em>{{ tuto.authors }}</em></p>
<p>Presented on {{ tuto.date }} at {{ tuto.conference }}</p>
<p>{{ tuto.description }}</p>
{% for link in tuto.links %}
<p><strong><a href="{{ link.url }}">{{ link.display }}</a></strong></p>
{% endfor %}

</li>
{% endfor %}

</ul>

## Old University Courses

I have been involved in the following courses.

<ul>

{% for course in site.data.oldcourselist %}
<li>
<p>{{ course.title}}, as a {{course.role}} ({{ course.date }})</p>
</li>

{% endfor %}

</ul>