---
layout: page-fullwidth
title: "Plantilla del post"
subheadline: "Ayuda"
teaser: "Qué debe contener un post"
permalink: "/tutopost/plantillapost/"
categories:
  - tutopost
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
Cuando quieras crear un post, debes asegurarte en rellenar los siguientes campos. Es posible que no sean todos.

Está página es un complemento de la ayuda ["Cómo crear un post"]({{ site.url }}/tutopost/crearpost/).

## Estructura de un post
Asgúrate que la página tenga esta estructura

~~~
---
layout: page
#
# Contenido
#
title: "Título"
subheadline: "Subtítulo"
teaser: "Descripción"
meta_description: "Palabras claves"
categories:
  - cat
tags:
  - tag
#
# Estilo
#
image:
  header: ""
  thumb: ""
  homepage: ""
  caption: ""
  url: ""
---
Cuerpo del texto
~~~

## Estructura de un post con una imagen de fondo

~~~
---
layout: page
#
# Contenido
#
title: "Título"
subheadline: "Subtítulo"
teaser: "Descripción"
meta_description: "Palabras claves"
categories:
  - cat
tags:
  - tag
#
# Estilo
#
image:
    title: title_image.jpg
    thumb: thumbnail_image.jpg
    homepage: header_homepage_13.jpg
    caption: Image by Phlow
    caption_url: "http://phlow.de/"
---
Cuerpo del texto
~~~


## Agradecimientos

La plantilla está basada en la [documentación de Jekyll](https://jekyllrb.com/docs/posts/).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
