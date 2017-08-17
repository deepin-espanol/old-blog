---
layout: page
subheadline:  "Manual"
title:  "Fondos de pantalla 1"
teaser: "Nuestros fondos de pantalla. Transiciones cortesía de <a href='http://foundation.zurb.com/docs/components/clearing.html'>Clearing Lightbox</a>."
categories:
    - manual
tags:
    - markdown
    - wallpapers
image:
   thumb: "gallery-example-1-thumb.jpg"
gallery:
    - image_url: gallery-example-1.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-2.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-3.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-4.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-5.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-6.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-7.jpg
      caption: Gran wallpaper por Unsplash.com
    - image_url: gallery-example-8.jpg
      caption: Gran wallpaper por Unsplash.com
---
Esta es la primera parte de nuestros *fondos de pantalla* basadas en paisajes. Por su puesto, lo puedes encontrar desde [unsplash](https://unsplash.com/) sin coste algo ni por pago de regalías.

{% include gallery %}

## Cómo crear un post con fondos de pantalla

Solo necesitas escoger una plantillas como `page` o `page-fullwidth` e incrustar dentro de la página `{% raw %}{% include gallery %}{% endraw %}`.

Para las imágenes:

1. Necesitarás obtener la de mayor resolución y nombrar *gallery-image.jpg*..
2. Y otra reducida (thumbnail) *gallery-image-thumb.jpg* y...
3. Coloca a ambas en la carpeta *images*.

Para definir los fondos escribe en el código de la página:

~~~
gallery:
    - image_url: gallery-image.jpg
~~~

Y establece una descripción adicional

~~~
gallery:
    - image_url: gallery-image.jpg
       caption: Starting Page with huge One Logo
~~~


{% include alert info='Gracias por visitar esta página. Compartir esta página es gratis como los fondos :)' %}


## Más sobre fondos de pantalla
{: .t60 }
{% include list-posts tag='wallpapers' %}



 [1]: http://foundation.zurb.com/docs/components/clearing.html
 [2]: http://foundation.zurb.com/docs/components/block_grid.html
