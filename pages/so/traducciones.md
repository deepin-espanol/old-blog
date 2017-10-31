---
layout: page-fullwidth
title: "Traduce Deepin"
subheadline: "Sistema operativo"
teaser: "Lista de traducciones."
header:
   image_fullwidth: "wallpaper.jpg"
permalink: "/traducciones/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.tags.traducciones %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Este listado de recomendaciones está relacionado a los títulos, palabras frecuentes y aproximaciones. Muchas veces usamos para la interfaz de Deepin, la página web o las marcas comerciales. Están etiquetadas como "traducciones", algunas páginas de <a href="{{ site.url }}{{ site.baseurl }}/anexos/">Anexos</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.

    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
