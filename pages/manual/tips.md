---
layout: page-fullwidth
show_meta: false
title: "Tips"
subheadline: "Consejos y más"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/tips/"
---
<div class="row t60">
    <div class="medium-6 columns b30">
      <ul>
          {% for post in site.categories.tips %}
          <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
          {% endfor %}
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
      Está categoría contiene páginas de ayuda que complementan al <a href="{{ site.url }}{{ site.baseurl }}/manual/">manual de usuario</a>. Algunos de ellos requieren de la <a href="{{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/">terminal</a> o <a href="{{ site.url }}{{ site.baseurl }}/anexos/dudas-tecnicas/">conocimientos sobre GNU/Linux</a>.

      Explora más en el <a href="{{ site.url }}{{ site.baseurl }}/blog/archive/">Archivo</a>, la <a href="{{ site.url }}{{ site.baseurl }}/introduccion/">Introducción</a> o la sección <a href="{{ site.url }}{{ site.baseurl }}/info/">Información</a>.
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
