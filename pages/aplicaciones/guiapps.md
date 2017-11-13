---
layout: page
title: "Listado de aplicaciones"
teaser: "El catálogo más amplio para tus actividades."
permalink: "/guiapps/"
header:
    image_fullwidth: "header_drop.jpg"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.guiapps %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Este es la lista de programas por uso etiquetadas como "guiapps", hija de la categoría <a href="{{ site.url }}{{ site.baseurl }}/apps/">Aplicaciones</a>. Si quieres ver las aplicaciones incluidas, <a href="{{ site.url }}{{ site.baseurl }}/escenciales/">visita esta página</a>.<br/>

      ¿Perdido(a)? Visita <a href="{{ site.url }}{{ site.baseurl }}/anexos/guiapps/">la guía principal</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
