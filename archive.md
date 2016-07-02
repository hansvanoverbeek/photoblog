---
layout: default
title: Archive
description: Een gesorteerd overzicht van de gepubliceerde posts
permalink: /archive/
---

 <h3 class="text-center">Blog Archief</h3>

 <main id="archive">

  <div class="archie-box">

   <h4>Categorie&euml;n</h4>

   <h5>Landschap</h5>
    <ul>
      {% for item in site.categories.landschap %}
       <li><span >{{ item.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a></li>  
      {% endfor %}     
    </ul>    

    <h5>Schepen</h5>
    <ul>
      {% for item in site.categories.schepen %}
       <li><span >{{ item.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a></li>  
      {% endfor %}     
    </ul>

     <h5>Planten</h5>
    <ul>
      {% for item in site.categories.planten %}
       <li><span >{{ item.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a></li>  
      {% endfor %}     
    </ul>

     <h5>Stadsgezicht</h5>
    <ul>
      {% for item in site.categories.stadsgezicht %}
       <li><span >{{ item.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a></li>  
      {% endfor %}     
    </ul>

     <h5>Diverse</h5>
    <ul>
      {% for item in site.categories.diverse %}
       <li><span >{{ item.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a></li>  
      {% endfor %}     
    </ul>
    </div>

  <div class="archive-box">
   <h4>Chronologisch</h4>
  {% for post in site.posts %}
  {% capture month %}{{ post.date | date: '%m%Y' }}{% endcapture %}
  {% capture nmonth %}{{ post.next.date | date: '%m%Y' }}{% endcapture %}

    {% if month != nmonth %}
    {% if forloop.index != 1 %}</ul>{% endif %}

  <h5>{{ post.date | date: '%B %Y' }}</h5>
  <ul>
    {% endif %}
    <li><span >{{ post.date | date: "%d/%m/%Y" }}&nbsp;&nbsp;</span><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>  
    {% endfor %}
  </ul>
  </div>

</main>
