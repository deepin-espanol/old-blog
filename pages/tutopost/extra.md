---
layout: page-fullwidth
title: "Código extra en posts"
subheadline: "Ayuda"
teaser: "Qué más puedes añadir en los posts"
permalink: "/tutopost/extra/"
categories:
  - tutopost
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


Además de añadir encabezados (detalles en [página Doc]({{ site.url }}/tutopost/extra/)), en *Deepin en Español* puedes añadir o incrustar multimedia como:


## Estilo en posts   {#styling}

Feeling Responsive offers lots of possibilities to style your articles. You can style your content in different ways. There are elements like subheadlines, feature images, header images, homepage images, meta data like categories and tags and many more.

### Anclas

Las anclas entrelazan a la página. Son bastante organizados.
`{#styling}`

### subheadlines

Si quieres añadir un línea debajo del encabezado, define al iniciar el texto como:

`subheadline:  "Subheadline"`

### Citas

Las citas son apropiadas para entrevistas o contenido de páginas web usa el siguiente código:

> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }


## Comentarios

Puedes usar comentarios con *Feeling Responsive* cortesía de Disqus. Si usas Disqus-Comments abre `config.yml` y establece en el `disqus_shortname`. [More on how to use Disqus ›](https://disqus.com/websites/)

Por defecto, están desactivados y puedes personalizar en `config.yml`. Para **activar comentarios** añade el código `comments: true` debajo de `layout: page`. 

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }




## Vídeos adaptables al tamaño

Con foundation los vídeos adaptables al tamaño (flexible) son fáciles. [More ›](http://foundation.zurb.com/docs/components/flex_video.html)

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/WoHxoz_0ykI" frameborder="0" allowfullscreen></iframe>
</div>

### Code to use for flexible videos

{% highlight html %}
<div class="flex-video">
  <iframe with video />
</div>
{% endhighlight %}


<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="">

## Crear una tabla de contenido
{: .t60}

Con el código pasador Kramdown puedes renderizar una tabla de contenido al post. Solo inserta el siguiente código antes de añadir párrafos. Más información en [»Automatic ›Table of Contents‹ Generation«](http://kramdown.gettalong.org/converter/html.html#toc).

### Versión Bare Bones
{% highlight html %}
### Table of Contents
*  Auto generated table of contents
{:toc}
{% endhighlight %}

### Versión panel Foundation

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

## Miga de pan

Para activar una miga de pan ([breadcrumbs](https://es.wikipedia.org/wiki/Miga_de_pan_(inform%C3%A1tica))), añade...

{% highlight html %}
breadcrumb: true
{% endhighlight %}


## Códigos listos para usar
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

### next-previous-post-in-category.html

Añade enlaces al anterior y siguiente post. En el front matter se añade.

~~~
{% raw %} {% include next-previous-post-in-category %}{% endraw %}
~~~


### improve_content

Útil para editar código fuente directamente similar a una wiki. Está inspirada en [Ben Balters Blog](http://ben.balter.com/).

~~~
{% raw %}{% include _improve_content.html %}{% endraw %}
~~~


### list-collection

Permite agrupar publicaciones que no están publicadas, de todas formas usa el siguiente código.

~~~
{% raw %}{% include list-collection collection='wordpress' %}{% endraw %}
~~~


### alert – Incrustar un aviso en la publicación

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

{% include alert info='<em>Feeling Responsive</em> is listed on <a href="http://jekyllthemes.org/">http://jekyllthemes.org</a>' %}

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
