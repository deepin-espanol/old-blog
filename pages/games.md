---
layout: page
title: "Juegos"
subheadline: "Listado para jugones"
teaser: "Lista de juegos compatibiles de Deepin."
permalink: "/games/"
header:
    image_fullwidth: "header_drop.jpg"
---

La lista de juegos va aquí. Llevan etiquetados como "juego".

<ul>
    {% for post in site.tags.juego %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
