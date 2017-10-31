---
layout: page-fullwidth
title: "Aplicaciones originales"
subheadline: "Aplicaciones "
teaser: "Las aplicaciones desarrolladas por Deepin."
permalink: "/games/"
header:
    image_fullwidth: "header_drop.jpg"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.originales %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      <ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      La lista de ⌨ aplicaciones desarrolladas por Deepin va aquí. Llevan etiquetados como "originales". Actualizamos desde <a href="https://www.deepin.org/es/original/">Deepin.org</a>. Es complementario a la categoría <a href="{{ site.url }}{{ site.baseurl }}/apps/">Aplicaciones</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
