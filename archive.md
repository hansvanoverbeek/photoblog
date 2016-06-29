---
layout: default
title: Archive
description: Een gesorteerd overzicht van de gepubliceerde posts
permalink: /archive/
---

<main id="archive">

  <h3>Blog Archive</h3>

  {% for post in site.posts %}
  {% capture month %}{{ post.date | date: '%m%Y' }}{% endcapture %}
  {% capture nmonth %}{{ post.next.date | date: '%m%Y' }}{% endcapture %}

    {% if month != nmonth %}
    {% if forloop.index != 1 %}</ul>{% endif %}

  <h4>{{ post.date | date: '%B %Y' }}</h4>
  <ul>
    {% endif %}
    <li><span >{{ post.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ post.url }}">{{ post.title }}</a></li>

{% endfor %}

<hr>
