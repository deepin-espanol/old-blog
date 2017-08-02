---
layout: page-fullwidth
title: "Tutorial para crear posts"
subheadline: "Ayuda"
teaser: "Haciendo artículos para principianes"
permalink: "/info/tutopost/crearpost/"
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
{% include alert text='Actualizado el 31 de julio de 2017. Es posible que sufran algunos cambios para casos específicos.' %}

## Qué es git y Jekyll

Los detalles puedes encontrar en [esta página]({{ site.url }}/tutopost/gityjekyll/).

## Primero: Clona desde un cliente git

Para empezar, usa una aplicación como [Gitcola](https://git-cola.github.io/) o la terminal.

~~~
git clone https://github.com/deepin-espanol/deepin-espanol.github.io.git
~~~

## Qué carpetas debo tocar

Como no hay interfaz web, desde tu gestor de archivos en el lugar:

* Las carpetas para páginas como " _drafts" para borradores, " _posts" para publicaciones en el blog y "pages" para páginas especiales; y
* La carpeta para las imágenes como "images".

### Preparación

1. Busca la carpeta * > _draft > ejemplo
2. Selecciona un archivo. Más detalles en la siguiente sección.
3. Pega a la carpeta * >_draft > mejorar
4. Realiza los retoques, comprueba si el código funciona correctamente.
5. Corta el archivo
6. Muévelo a post > [carpeta]. Siendo carpeta, el manual, blog o tips.

### Qué debe contener un post

Cuando creas un archivo asegúrate que contenga:

* title: "" (título)
* subheadline: "" (subtítulo)
* teaser: "" (adelanto)
* categories: (como manual, blog, app o tip)
* tags: (etiqueta)

### Código Markdown

El lenguaje que aplicamos es [Markdown](https://es.wikipedia.org/wiki/Markdown) por ser fácil de aprender, casi lo mismo a una wiki.

* Escribe `*cursiva*` sale *cursiva*
* Escribe `**negrita**` sale **negrita**
* Escribe  `[Texto del enlace aquí](URL "Título del enlace")` y creas un enlace
* Escribe `![Texto alternativo](URL "Título de la imagen")` y creas una imagen

Para aprender todas las posibilidades visita [Códigos permitidos en Markdown]({{ site.url }}/tutopost/doc/). Si quieres editar desde la web, te presentamos JBT](https://jbt.github.io/markdown-editor/) o [Diliger](http://dillinger.io/). 

## Publicar vía git

Pare realizar un commit o parche, asegúrate que hayas realizado modificaciones como los nuevos archivos que has creado.

Primero: Una vez realizado el parche tienes dos opciones:

8. Haz un push en la branch o rama "[usuario]-post".
9. Si deseas pueds añadir más parches para corregir algunos percances.
10. Cuando está listo, tendrás que hacer la orden "merge".

En lugar de "merge", desde la web de Github:

10. Pide un "pull request", o solicitud para aplicar los parches, a la rama central.
11. Una vez revisado en la sección Issues, se aplican los parches y se elimina la rama obsoleta.

Segundo: O el más directo y **no recomendado**.

8. Hacer un push en la rama "master".
9. Si hay conflictos por aplicar paches antes de tiempo, es mejor realizar un "fetch" de la rama que vas a aplicar.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }


### Subir imágenes al sitio web

Este portal te permite subir imágenes a partir de la carpeta "images". Recomandamos comprimir lo máximo posible para que el navegador cargue más rápido y no desperdicie ancho de banda

## Anexo: Carpetas y actualizaciones
En caso que quieras actualizar Feeling Responsive tendrás que tomar en cuenta:

* La configuración propia como la carpeta " _data" y el archivo " _config.yml", esos no se modifican;
* Los archivos para que el servidor interprete código como "Gemfile", se puede modificar si fuera necesario;
* Las carpetas base como " _includes" para HTML, " _layouts" para traducir los posts, " _sass" para el framework Foundation si se deben actualizar;
* La carpeta "assets" para las liberías Javascript y CSS requiere atención, exepcto "img" que posee los iconos propios y no se deben perder

### Porqué usamos Jeryll

* Galería, vídeos, tipografía
* 100% GitHub Pages friendly
* Easy editable navigation, footer and social media links
* Language Ready – just translate one file.
* Lots of possibilities to customize it to your needs
* Lots of different headers
* Various post formats to let your content shine
* Uses Jekyll 3.0
* Multiple possibilities to use images in different ways
* Fine typography
* Play Video and Audio with [Mediaelement.js]({{ site.url }}/tutopost/mediaelement/)

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

La fuente oficial de Git proviene del [manual de 2014](https://git-scm.com/book/es/v2).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
