---
layout: page-fullwidth
title: "Tutorial para crear posts"
subheadline: "Ayuda"
teaser: "Haciendo artículos para principianes"
permalink: "/info/tutopost/"
header:
   image_fullwidth: "header_roadmap_2.jpg"
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

## Qué es Jekyll

Para que cada publicación en *Deepin en Español* sea rápida, colaborativa y seguro, tenemos que desarrollar un mecanismo. Ese mecanismo para elaborar la página web y los contenidos se llama [Jekyll](https://jekyllrb.com/).

Jekyll es similar a Wordpress, Joomla o Blogger. La ventaja es, que al ser de código abierto, su facilidad de uso tipo rompecabezas. El requisito principal es un servidor que permita ejecutar archivos escritos en [Ruby](https://es.wikipedia.org/wiki/Ruby).

## Qué carpetas hay

Sin llegar a los detalles técnicos, vamos a agrupar las carpetas y archivos en lo siguiente:

* La configuración propia como la carpeta " _data" y el archivo " _config.yml"
* Los archivos para que el servidor interprete código como "Gemfile"
* Las carpetas base como " _includes" para HTML, " _layouts" para traducir los posts, " _sass" para el framework Foundation y "assets" para las liberías Javascript y CSS.
* Las carpetas para páginas como " _drafts" para borradores, " _posts" para publicaciones en el blog y "pages" para páginas especiales.

Nosotros nos enfocaremos en la última agrupación.

## Paso para crear un post

Puedes crear desde cero. Pero te damos los pasos más fáciles

1. Busca la carpeta * > _draft > ejemplo
2. Selecciona un archivo. Más detalles en la siguiente sección.
3. Pega a la carpeta * >_draft > mejorar
4. Realiza los retoques, comprueba si el código funciona correctamente.
5. Corta el archivo
6. Muévelo a post > [carpeta]. Siendo carpeta, el manual, blog o tips.
7. Realiza un commit o parche.

Una vez realizado el parche tienes dos opciones:

8. Haz un push en la branch o rama "[usuario]-post".
9. Si deseas pueds añadir más parches para corregir algunos percances.
10. Cuando está listo, tendrás que pedir un "pull request", o solicitud para aplicar los parches, a la rama central.
11. Una vez revisado en la sección Issues, se aplican los parches y se elimina la rama obsoleta.

O el más directo y **no recomendado**.

8. Hacer un push en la rama "master".
9. Si hay conflictos por aplicar paches antes de tiempo, es mejor seguir los pasos de arriba.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Aprender a usar Markdown

El lenguaje que aplicamos es [Markdown](https://es.wikipedia.org/wiki/Markdown) por ser fácil de aprender, casi lo mismo a una wiki.

* Escribe `*cursiva*` sale *cursiva*
* Escribe `**negrita**` sale **negrita**
* Escribe  `[Texto del enlace aquí](URL "Título del enlace")` y creas un enlace
* Escribe `![Texto alternativo](URL "Título de la imagen")` y creas una imagen

Si quieres editar Markdown, te presentamos JBT](https://jbt.github.io/markdown-editor/) o [Diliger](http://dillinger.io/).

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
