---
layout: page-fullwidth
show_meta: false
title: "Etiqueta Programación"
subheadline: "Programando en Deepin con la API y herramientas de desarrollo."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/programacion/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.desarrollo %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Esta etiqueta contiene páginas sobre programación en Deepin Linux como el diseño de interfaces de usuario, paquetes Flatpak y lenguaje Qt. Forma parte de la categoría <a href="{{ site.url }}{{ site.baseurl }}/tecnico/">Técnico</a>).

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
