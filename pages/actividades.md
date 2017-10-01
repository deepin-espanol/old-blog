---
layout: page
title: "Formas de participar"
subheadline: "Info"
teaser: "Ayúdanos a mejorar Deepin recibiendo comentarios o aportando mejoras."
header:
   image_fullwidth: "header_roadmap_3.jpg"
permalink: "/participa/"
---

<img src="{{ site.urlimg }}Fondo 3d Logo comunidad.png" alt="">

Actividades que puedes hacer:

<ul>
    {% for post in site.categories.actividades %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
