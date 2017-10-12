---
layout: page-fullwidth
title: "Crear una página de fondos de pantalla"
subheadline: "Ayuda"
teaser: "Cómo elaborar una selección de fondos para Deepin"
tags:
    - tutopost
categories:
    - tecnico
breadcrumb: true
show_meta: false
header:
   image_fullwidth: "edition.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Índice**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">

Te mostramos en unos pasos que puedes hacer para perfeccionar este protal web. Necesitarás conocer un poco el funcionamiento y sentido común.

## Pasos
Solo necesitas escoger una plantillas como `page` o `page-fullwidth` e incrustar dentro de la página `{% raw %}{% include gallery %}{% endraw %}`.

Para las imágenes:

1. Necesitarás obtener la de mayor resolución y nombrar *gallery-image.jpg*.
2. Subir a un proveedor de Internet para subir como Imgur.
3. Realiza una miniatura (thumbnail) *gallery-image-thumb.jpg* y...
4. Sube la miniatura en la carpeta *images* de la página web.

{% include alert info='El motivo porque no subimos el fondo de mayor de resolución es para evitar abusar el ancho de banda del sitio web.' %}

## Pasos para elaborar un post

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

## Lectura adicionales
* ["Git en Atom"]({{ site.url }}/tips/gitatom/).
* [Cuerpo del post]({{ site.url }}/tutopost/cuerpopost/).


</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
