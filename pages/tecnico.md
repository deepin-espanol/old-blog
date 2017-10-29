---
layout: page-fullwidth
show_meta: false
title: "Información técnica"
subheadline: "API, herramientas de desarrollo de Deepin... y Deepin en Español."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/tecnico/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.tecnico %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Esta categoría contiene herramientas de desarrollo para Deepin Linux como la interfaz de usuario, paquetes Flatpak y la página de desarrollo del blog (alias <a href="{{ site.url }}{{ site.baseurl }}/tutopost/">Tutopost</a>).

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
