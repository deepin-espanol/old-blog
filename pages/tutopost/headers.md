---
layout: page
subheadline: "Header"
sitemap: false
title: "¡Este es la cabecera!"
teaser: "Esas son las opciones para dar estilo a la cabecera de esta página web. <em>Feeling Responsive</em> usa <a href='http://srobbin.com/jquery-plugins/backstretch/'>Backstretch by Scott Robin</a> para expandirla de izquierda a derecha. El ancho solicitado es de 1600 píxeles o superior con un ratio de 16:9, 21:9 o 2:1."
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/headers/"
---
Mira, estas son las aplicaciones:
<ul>
    {% for post in site.tags.apps %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
