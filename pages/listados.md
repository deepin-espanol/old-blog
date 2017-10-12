---
layout: page
show_meta: false
title: "Listados"
subheadline: "Recopilaciones de herramientas, fondos de pantalla y anexos."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/listados/"
---
<ul>
    {% for post in site.categories.listados %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}/blog/archive/).
