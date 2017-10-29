---
layout: page-fullwidth
show_meta: false
title: "Noticias"
subheadline: "Publicaciones de nuestra comunidad"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/noticias/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.noticias %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Esta categoría recopila las noticias publicadas por Deepin en Español. Las últimas en publicarse son mostradas en la página principal.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
