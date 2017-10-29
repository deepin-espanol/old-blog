---
layout: page-fullwidth
title: "Juegos"
subheadline: "Listado para jugones"
teaser: "Lista de juegos compatibiles de Deepin."
permalink: "/games/"
header:
    image_fullwidth: "header_drop.jpg"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.juego %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      La lista de 🎮 juegos va aquí. Llevan etiquetados como "juego". Algunos juegos lo puedes encontrar en <a href="{{ site.url }}{{ site.baseurl }}/apps/steam">Steam</a>. Es complemento de la categoría <a href="{{ site.url }}{{ site.baseurl }}/apps/">Aplicaciones</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
