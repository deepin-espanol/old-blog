---
layout: page-fullwidth
title: "Código de formato en posts"
subheadline: "Ayuda"
teaser: "El repertorio de opciones que puedes incorporar a las publicación"
tags:
    - tutopost
categories:
    - tecnico
breadcrumb: true
show_meta: false
header:
   image_fullwidth: "header_roadmap_2.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Tabla de contenidos**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
{% include _improve_content.html %}

## Formato de página o post   {#formats}

*Deepin en español* usa el tema **Feeling Responsive* para realizar diferentes formatos en las página web. Esta sirve de guía, incluyendo una explicación más detallada.

Nota: En inglés se conoce como front matter que es mostrada a lado de categorías o etiquetas.

Nota 2: Otros detalles encontrarás en [página Extra]({{ site.url }}/tutopost/extra/).

### Page/Post
El formato página/post no tiene texto lateral por defecto, su contenido está centrado y debajo de ella conteiene metadatos como categorías, etiquetas, fecha de creación y autor.

Al comenzar la edición añade el código: `layout: page`

### Page/Post con lateral izquierda o derecho
Para mostrar un lateral, añade `sidebar: left` o `sidebar: right` y en el front matter, y *vaya, es todo*. El contenido del lateral proviene del archivo `_includes/sidebar`.


### Page/Post con o sin metadatos
Al mostrar metadatos como categorías, etiquetas y otros, incluye el código `show_meta: true`. Viene por defecto, dependiendo de la página de configuración `_config.yml`. De lo contrario, para ocultar reemplaza a `show_meta: false`.


### Page Full Width
Las páginas panorámicas o de ancho completo son apropiadas para añadir tablas o galerías. Otros detalles encontrarás en [foundation grid system](http://foundation.zurb.com/docs/components/grid.html).

En front matter usa: `layout: page-fullwidth`


### Frontpage
Este código es especial, porque permite añadir tres *widgets* en el encabezado, además de descripción y enlaces. Es usada en la [página central]({{ site.url }}{{ site.baseurl }}) del sitio web.

En front matter usa: `layout: frontpage`


### Video
Si quieres añadir vídeos en lugar de imágenes, tenemos una plantilla especial. Cambia a un fondo oscuro y da presentación al vídeo a pantalla completa.

En front matter usa: `layout: video`

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Personalizar la página

## Imágenes: Principal, miniatura e inicio {#images}

Recomendado para añadir noticias.


### Imagen principal

~~~
image:
    title: image.jpg
~~~


### Miniatura

Tienen un tamaño de 150x150 pixels. Se define como:

~~~
image:
    thumb: thumbnail_image.jpg
~~~


### Imagen de inicio

Como un ancho mínimo 970 pixels, se añade una imagen panorámica al señalar un post en la página principal. Defínelo como:

~~~
image:
    homepage: header_homepage_13.jpg
~~~



### Subtítulo con URL

Idel para dar crédito al autor de la imágen o detallar más. Escribe como:

~~~
image:
    title: header_image.jpg
    caption: Image by Phlow
    caption_url: "http://phlow.de/"
~~~

### Ejemplo para añadir imágenes de encabezado al artículo

~~~
image:
    title: title_image.jpg
    thumb: thumbnail_image.jpg
    homepage: header_homepage_13.jpg
    caption: Image by Phlow
    caption_url: "http://phlow.de/"
~~~


<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }


## Módulos Javascript/Foundation

Esta sección solo está enfocado en optimizar *Feeling Responsive*, ya que tiene módulos que hacen cargar más rápido de lo normal.

También se añade otro módulo javascript: [`backstretch`](http://srobbin.com/jquery-plugins/backstretch/) de Scott Robbin. Esos módulos son usados en el tema junto a la librería reducida `javascript.min.js`.

~~~
/foundation/bower_components/foundation/js/vendor/jquery.js'
/foundation/bower_components/foundation/js/vendor/fastclick.js'
/foundation/bower_components/foundation/js/foundation.accordion.js'
/foundation/bower_components/foundation/js/foundation.clearing.js'
/foundation/bower_components/foundation/js/foundation.dropdown.js'
/foundation/bower_components/foundation/js/foundation.equalizer.js'
/foundation/bower_components/foundation/js/foundation.magellan.js'
/foundation/bower_components/foundation/js/foundation.topbar.js'
/foundation/js/jquery.backstretch.js'
~~~

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
