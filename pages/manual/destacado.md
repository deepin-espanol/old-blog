---
layout: page-fullwidth
show_meta: false
title: "Destacado"
subheadline: "Lo resaltado del manual"
header:
   image_fullwidth: "hot.jpg"
permalink: "/tips/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.destacado %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Estas son las páginas etiquetadas con "Destacado". Mayormente son soluciones más frecuentes o acciones en situaciones de riesgo.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
