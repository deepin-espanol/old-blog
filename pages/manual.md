---
layout: page
show_meta: false
title: "El manual"
subheadline: "Aprende a usar Deepin"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/manual/"
---
<ul>
    {% for post in site.categories.manual %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
