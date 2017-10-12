---
layout: page
show_meta: false
title: "Información técnica"
subheadline: "API, herramientas de desarrollo de Deepin... y Deepin en Español."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/tecnico/"
---
Esta categoría contiene herramientas de desarrollo para Deepin Linux, interfaz de usuario. También fusionamos con el [Tutopost]({{ site.url }}{{ site.baseurl }}/tutopost/).
<ul>
    {% for post in site.categories.listados %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Ir al [Archivo]({{ site.url }}{{ site.baseurl }}/blog/archive/).
