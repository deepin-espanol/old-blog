---
layout: page
show_meta: false
title: "Dudas frecuentes"
subheadline: "La lista de dudas para todos los usuarios"
header:
   image_fullwidth: "hot.jpg"
permalink: "/tips/"
---
Está listado contiene páginas relacionadas con "Dudas". A diferencia de los tips, están estructuradas en preguntas y respuestas. Es similar a preguntas más frecuentes.

<ul>
    {% for post in site.tags.dudas %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}/blog/archive/).
