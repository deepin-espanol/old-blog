---
layout: page
show_meta: false
title: "Noticias"
subheadline: "Publicaciones de nuestra comunidad"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/blog/noticias/"
---
<ul>
    {% for post in site.categories.design %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
