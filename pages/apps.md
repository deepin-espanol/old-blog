---
layout: page
title: "Aplicaciones"
subheadline: "Nuestro listado"
teaser: "Lista de aplicaciones, juegos y agregados para Deepin."
permalink: "/apps/"
header:
    image_fullwidth: "header_drop.jpg"
---

En Deepin comentamos y comprobamos varias aplicaciones. También incluímos [juegos]({{ site.url }}/games/) y [sets de iconos]({{ site.url }}/icons/)

Publicaciones:
<ul>
    {% for post in site.categories.manual %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
