---
title: "Quentin De Coninck - Teaching"
layout: textlay
excerpt: "Quentin De Coninck -- Teaching"
sitemap: false
permalink: /teaching/
---

# Teaching

My teaching contributions fall into two categories.
On the one hand, I have contributions to several tutorials that have been presented during academic conferences.
On the other hand, I am involved in the organization of University courses.

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

## University Courses

I have been involved in the following courses.

<ul>

{% for course in site.data.courselist %}
<li>
<p>{{ course.title}}, as a {{course.role}} ({{ course.date }})</p>
</li>

{% endfor %}

</ul>