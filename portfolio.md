---
layout: default
title: Portfolio
description: De portfolio pagina bevat links naar galeries die mijn belangrijkste thema's bevattten. The portfolio page contains links to the main galleries.
---

<h3 class="portfolio-header">{{ page.title }}</h3>

<section class="portfolio-container">

  <h4>Een selectie van themas</h4>

   <p>Thema&apos;s die mij in het bijzonder inspireren. Iedere link leidt naar een galerie met foto's van dat onderwerp.</p>
   <p>
     Themes in particular inspiring to me. Each link leads to a corresponding gallery.
   </p>

   <hr>
   
   {% for item in site.themas %}

    <li>
     <a href="{{site.baseurl}}/{{ item.url }}">{{ item.title }}
     <img src="{{ site.baseurl}}/{{ item.image_path }}" alt="{{ item.title }}">
     </a>
    </li>

   {% endfor %}

</section>
