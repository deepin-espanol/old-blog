---
layout: page-fullwidth
title: "Cuerpo del post"
subheadline: "Ayuda"
teaser: "Qué más puedes añadir en los posts"
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

Además de añadir encabezados, detalles en [la página correspondiente]({{ site.url }}{{ site.baseurl }}/tecnico/encabezadopost/), en *Deepin en Español* no basta escribir sino decorar con imágenes, vídeos y más.

{% include alert success='Esta página es un extracto de la serie de tutoriales, <a href="/tutopost">Tutopost</a>, para desarrollo en Jekyll' %}

Nota: Está página es un complemento de la ayuda ["Cómo crear un post desde Atom"]({{ site.url }}{{ site.baseurl }}/tecnico/crearpost/), mientras que los más avanzados se guiarán en [la página dedicada]({{ site.url }}{{ site.baseurl }}/tecnico/crearpost/).

## Básico
### Vídeos

Con foundation los vídeos adaptables al tamaño (flexible) son fáciles. [Más info ›](http://foundation.zurb.com/docs/components/flex_video.html)

Arriba el código, abajo el resultado.

{% highlight html %}
<div class="flex-video">
  <iframe with video />
</div>
{% endhighlight %}

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/WoHxoz_0ykI" frameborder="0" allowfullscreen></iframe>
</div>

### Imágenes

Arriba el código, abajo el resultado.

{% highlight html %}
<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="">
{% endhighlight %}

<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="">

### Enlaces internos

Puedes hacer un enlace interno sin escribir la URL del página es de la siguiente manera:

~~~
{% raw %}[titulo link]({{ site.url }}{{ site.baseurl }}/cat/titulo/){% endraw %}
~~~

## Código adicional {#adicional}

Feeling Responsive permite a las páginas, de la siguiente forma

### Crear una tabla de contenido
{: .t60}

Cuando hay varias secciones en la publicación, es necesario crear una tabla de contenido o índice.

Más información en [»Kramdown«](http://kramdown.gettalong.org/converter/html.html#toc).

El más sencillo y recomendado es de Bare Bones:
{% highlight html %}
### Table of Contents
*  Auto generated table of contents
{:toc}
{% endhighlight %}

Puedes hacer más complejo con el formato de Foundation:

{% highlight html %}
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
{% endhighlight %}
<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

### Anclas

Las anclas sirven para enlazar partes específicas a la página. Basta escribir
`{#nombre}` El numeral indica el nombre de esa ancla.

### Citas

Las citas son apropiadas para entrevistas o extractos de páginas web. Usa el siguiente código:

> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

~~~
{% highlight html %}
Código
{% endhighlight %}
~~~

## Avisos

### Mejorar contenido

Llamado ´improve_content´. Útil para editar código fuente directamente similar a una wiki. Está inspirada en [Ben Balters Blog](http://ben.balter.com/).

~~~
{% raw %}{% include _improve_content.html %}{% endraw %}
~~~

### Columnas

Para crear una columna, [debes usar las etiquetas "div" y usar la clase "row"]({{ site.url }}{{ site.baseurl }}/tecnico/columnas/).

### Incrustar un aviso en la publicación

Ese método es útil para avisar a los usuarios. Por favor, no añadas `.html` para evitar errores. Tienes cinco tipos de avisos: `warning`, `info`, `success`, `alert` y `text`.

~~~
{% raw %}{% include alert warning='This is a warning.' %}
{% include alert info='An info box.' %}
{% include alert success='Yeah, you made it!' %}
{% include alert alert='Danger!' %}
{% include alert terminal='jekyll -serve' %}
{% include alert text='Just a note!' %}{% endraw %}
~~~

{% include alert warning='This is a warning.' %}
{% include alert info='An info box.' %}
{% include alert success='Yeah, you made it!' %}
{% include alert alert='Danger!' %}
{% include alert terminal='jekyll -serve' %}
{% include alert text='Just a note!' %}

Si es posible usa la etiqueta `<html>` como en la siguiente demostración.

~~~
{% raw %}{% include alert info='<em>Feeling Responsive</em> is listed on <a href="http://jekyllthemes.org/">http://jekyllthemes.org</a>' %}{% endraw %}
~~~

{% include alert info='<em>Feeling Responsive</em> está listado <a href="http://jekyllthemes.org/">http://jekyllthemes.org</a>' %}

## Código líquido
{: .t60}

Puedes añadir códigos especiales Markdown (llamados Liquid code).

### Lista de publicaciones

Son bastante útiles para añadir un listado de publicaciones filtrado por:

- entries › entradas máximas
- offset › entradas omitidas desde el inicio
- category › define **una** categoría para mostrar dichas entradas

Así funciona si quiero listar las noticias desde el segundo hasta el cuarto:

~~~
{% raw %}{% include list-posts entries='3' offset='1' category='noticias' %}{% endraw %}
~~~

### Lista colección

Permite incrustar un listado publicaciones como páginas.

~~~
{% raw %}{% include list-collection collection='wordpress' %}{% endraw %}
~~~

### Enlace Anterior y Siguiente

Llamado `next-previous-post-in-category.html`. Añade enlaces al anterior y siguiente post. En el front matter se añade.

~~~
{% raw %} {% include next-previous-post-in-category %}{% endraw %}
~~~


<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
