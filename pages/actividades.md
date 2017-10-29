---
layout: page-fullwidth
title: "Formas de participar"
subheadline: "Info"
teaser: "Ayúdanos a mejorar Deepin recibiendo comentarios o aportando mejoras."
header:
   image_fullwidth: "header_roadmap_3.jpg"
permalink: "/actividades/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.actividades %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Está categoría muestra las actividades que realizamos en Deepin en Español. Si tienes tiempo, y habilidad si es posible, recurre a cualquiera de ellas.

      <img src="{{ site.urlimg }}Fondo 3d Logo comunidad.png" alt="">

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
