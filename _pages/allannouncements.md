---
title: "BRICC@MICS Announcements"
layout: textlay
excerpt: "BRICC@MICS Announcements."
sitemap: false
permalink: /allannouncements.html
---

# Announcements

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline | markdownify}}</em></p>
{% endfor %}
