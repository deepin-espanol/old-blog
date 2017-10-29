---
layout: page-fullwidth
title: "Iconos"
subheadline: "Un listado"
teaser: "Lista de Iconos Deepin."
permalink: "/icons/"
header:
    image_fullwidth: "header_drop.jpg"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.iconos %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      La 🖌 lista de iconos está aquí. Son aplicaciones etiquetadas como "iconos". Para cambiar los iconos, revisa la <a href="{{ site.url }}{{ site.baseurl }}/manual/temas/">página del Manual</a>. Es complemento de la categoría <a href="{{ site.url }}{{ site.baseurl }}/apps/">Aplicaciones</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
