---
layout: page-fullwidth
show_meta: false
title: "Etiqueta Desarrollo"
subheadline: "API y herramientas de desarrollo de Deepin."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/desarrollo/"
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
      Esta etiqueta contiene información de desarrollo para Deepin Linux como la interfaz de usuario, paquetes Flatpak. Forma parte de la categoría <a href="{{ site.url }}{{ site.baseurl }}/tecnico/">Técnico</a>).

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
