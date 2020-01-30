---
title: "News"
layout: textlay
excerpt: "Quentin De Coninck's Activities."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
