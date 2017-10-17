---
layout: page
show_meta: false
title: "Destacado"
subheadline: "Lo resaltado del manual"
header:
   image_fullwidth: "hot.jpg"
permalink: "/tips/"
---
Estas son las páginas etiquetadas con "Destacado". Mayormente son soluciones más frecuentes o acciones en situaciones de riesgo.

<ul>
    {% for post in site.tags.destacado %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}/blog/archive/).
