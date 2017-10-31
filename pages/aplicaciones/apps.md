---
layout: page-fullwidth
title: "Aplicaciones"
subheadline: "Nuestro listado"
teaser: "Lista de aplicaciones, juegos y agregados para Deepin."
permalink: "/apps/"
header:
    image_fullwidth: "header_drop.jpg"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.apps %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      En Deepin te explicamos las aplicaciones que puedes instalar en Deepin y comentamos las posibilidades que puedes hacer con ella. También incluímos <a href="{{ site.url }}{{ site.baseurl }}/games/">juegos</a>, <a href="{{ site.url }}{{ site.baseurl }}/icons/">sets de iconos</a> y <a href="{{ site.url }}{{ site.baseurl }}/originales/">aplicaciones propias de Deepin</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
