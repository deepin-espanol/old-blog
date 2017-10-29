---
layout: page-fullwidth
show_meta: false
title: "Anexos"
subheadline: "Recopilaciones de herramientas, fondos de pantalla y anexos."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/anexos/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.anexos %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Esta categoría contiene páginas que anexan las categorías <a href="{{ site.url }}{{ site.baseurl }}/manual/">Manual</a> y <a href="{{ site.url }}{{ site.baseurl }}/tips/">Tips</a>. Están las dudas frecuentes, fondos de pantalla o listas de apoyo.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
