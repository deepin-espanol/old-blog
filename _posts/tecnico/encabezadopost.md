---
layout: page-fullwidth
title: "Encabezado del post"
subheadline: "Ayuda"
teaser: "Qué encabezado debe tener el post"
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
Si es tu primera vez que crearás un post, no te será complicado hacer desde cero.

Lo primero que hacemos es elaborar una página llamada "Hola mundo". Esa base nos servirá para elaborar una base. Tienes algunos campos para rellenar.

El siguiente paso es [que más incluir al post]({{ site.url }}{{ site.baseurl }}/tecnico/extra/).

Nota: Está página es un complemento de la ayuda ["Cómo crear un post desde Atom"]({{ site.url }}{{ site.baseurl }}/tecnico/crearpost/), mientras que los más avanzados se guiarán en [la página dedicada]({{ site.url }}{{ site.baseurl }}/tecnico/crearpost/).

## Estructura de un post
Al crear un archivo 12-12-titulo.md, tendrás que presentar el título y otras partes para mostrar en la publicación (categorías y etiquetas).

~~~
---
layout: page
#
# Contenido
#
title: "Hola mundo"
subheadline: "Subtítulo"
teaser: "Descripción"
meta_description: "Palabras claves"
categories:
  - tutoriales
tags:
  - mitag
#
# Estilo
#
---
Cuerpo del texto
~~~

### Con una imagen de fondo

Eso es opcional, añade una imagen para decorar el contenido. El resultado sería [decorativo]({{ site.url }}{{ site.baseurl }}/header/).

~~~
---
layout: page
#
# Contenido
#
title: "Hola mundo"
subheadline: "Subtítulo"
teaser: "Descripción"
meta_description: "Palabras claves"
categories:
  - tutoriales
tags:
  - mitag
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

### Vídeo de fondo
También puedes usar una vídeo de fondo. Muy adecuado a presentar una grabación sin recurrir demasiado al texto.

~~~
---
layout: video
#
# Contenido
#
title: "Hola mundo"
subheadline: "Subtítulo"
teaser: "Descripción"
meta_description: "Palabras claves"
categories:
  - tutoriales
tags:
  - mitag
  - video
#
# Estilo
#
iframe: "<iframe width='970' height='546' src='//www.youtube.com/embed/12345678' frameborder='0' allowfullscreen></iframe>"
video:
    embedURL: ""
    contentURL: ""
    thumbnailUrl: ""
---
Cuerpo del texto
~~~

## Extra

### subheadlines

Si quieres añadir un línea debajo del encabezado, define al iniciar el texto como:

`subheadline:  "Subheadline"`

### Miga de pan

Para añadir una miga de pan o [breadcrumbs](https://es.wikipedia.org/wiki/Miga_de_pan_(inform%C3%A1tica)), añade:

{% highlight html %}
breadcrumb: true
{% endhighlight %}

### Comentarios

Puedes usar comentarios con *Feeling Responsive* cortesía de Disqus. Si usas Disqus-Comments abre `config.yml` y establece en el `disqus_shortname`. [Sitio web de Disqus ›](https://disqus.com/websites/)

Por defecto, están desactivados y puedes personalizar en `config.yml`. Para **activar comentarios** añade el código `comments: true` debajo de `layout: page`.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/cuerpopost/">Ver información del cuerpo del post ›</a>

## Agradecimientos

La plantilla está basada en la [documentación de Jekyll](https://jekyllrb.com/docs/posts/).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
