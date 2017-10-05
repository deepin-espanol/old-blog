---
layout: page
title: "Iconos"
subheadline: "Un listado"
teaser: "Lista de Iconos Deepin."
permalink: "/icons/"
header:
    image_fullwidth: "header_drop.jpg"
---

La lista de iconos está aquí. Son aplicaciones etiquetadas como "iconos". Para cambiar los iconos, revisa la [página del Manual]({{ site.url }}{{ site.baseurl }}/manual/temas/).

<ul>
    {% for post in site.tags.iconos %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}/blog/archive/).
