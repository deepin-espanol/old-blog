---
layout: page-fullwidth
show_meta: false
title: "El manual"
subheadline: "Aprende a usar Deepin"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/manual/"
---

<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.manual %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Está categoría contiene publicaciones del manual de usuario como el uso de las aplicaciones de Deepin, explicaciones de sus funciones principales o los puntos básicos que debes saber.

      Ejemplos: Descarga e Instalación, Primeros pasos, Centro de control, Aplicaciones exclusivas de Deepin, Deepin Store, Arranque dual, Instalar controladores, entre otros.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.  
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
