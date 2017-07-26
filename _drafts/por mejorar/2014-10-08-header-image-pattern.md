---
layout: page
title:  "Imagen de encabezado con patrones"
subheadline:  "Tip Markdown"
teaser: "Usando Feeling Responsive te permite usar tipos de encabezados como se muestra este ejemplo con patrones."
categories:
    - tips
tags:
    - markdown
    - imagen
    - patrones
header:
    image: header_unsplash_2-970x.jpg
    pattern: pattern_concrete.jpg
    caption: Este es una descripción de la imagen de cabecera con un enlace
    caption_url: https://unsplash.com/
---
Es fácil de hacer. Define Just define in la cabecera una imagen y una imagen patrón. En lugar de un patrón puedes usar un color sólido. Echa un vistazo a [example with a background color]({{ site.url }}{{ site.baseurl }}/tips/header-image-color/).
<!--more-->

## Front Matter Code

~~~
header:
    image:  "header_unsplash_2-970x.jpg"
    pattern:  "pattern_concrete.jpg"
    caption: This is a caption for the header image with link
    caption_url: https://unsplash.com/
~~~



### All Header-Styles 
{: .t60 }

{% include list-posts tag='header' %}
