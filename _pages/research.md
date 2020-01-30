---
title: "Quentin De Coninck - Research"
layout: textlay
excerpt: "Quentin De Coninck -- Research"
sitemap: false
permalink: /research/
---

# Research

My research interests include multipath transport protocols and system architecture.
I also strive to provide reproducible results and release my softwares under open-source licenses.

# Publications

## Highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.be/citations?user=2akL5ySI3O0C&hl=en))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive img-margin" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List

Our DIAL institutional library gives access to pre-print of my papers.


<iframe src="https://dial.uclouvain.be/DialExport/Portail?method=keyword&amp;type=classic&amp;report=true&amp;book=true&amp;patent=true&amp;preprint=true&amp;conferencePaper=true&amp;journalArticle=true&amp;bookChapter=true&amp;thesis=true&amp;workingPaper=true&amp;sort=date&amp;sortType=desc&amp;author=De+Coninck%2C+Quentin" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true" width="100%" height="3600" frameborder="0"></iframe>