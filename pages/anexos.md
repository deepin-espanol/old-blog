---
layout: page
show_meta: false
title: "Anexos"
subheadline: "Recopilaciones de herramientas, fondos de pantalla y anexos."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/anexos/"
---
Esta categoría contiene páginas que anexan las categorías Manual y Tips.
<ul>
    {% for post in site.categories.anexos %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}/blog/archive/).
