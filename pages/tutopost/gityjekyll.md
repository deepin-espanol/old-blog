---
layout: page-fullwidth
title: "Tutorial para crear posts"
subheadline: "Ayuda"
teaser: "Haciendo artículos para principianes"
permalink: "/tutopost/gityjekyll/"
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

## Qué es git

Imagínate que es similar a Wikipedia. [Git](https://es.wikipedia.org/wiki/Git) es un sistema de control de versiones creado por Linus Torvalds. Los cambios principales están desarrollados en una rama llamada "master" que se puede bifurcar a otras menores para realizar cambios y revisarlos antes de aplicar a la principal.

En git, usamos órdenes para actualizar la página web (o también el código fuente de un programa) como :
* Las más importantes son **fetch** para descargar la última versión en línea.
* Para definir el cambio llamamos a **commit** (parche/ar) y para subir usamos **push**. Si cometemos un error, puedes revertir con **revert**.
* Para ramificaciones tienes **merge [nombre de rama]** para fusionar los cambios desde una rama menor a la principal y **pull** para ejecutar "fetch" y "merge" a la vez.

Nos enfocaremos en los dos primeros de la lista.

La mayoría de órdenes son de la terminal; no obstante, te recomendamos usar aplicaciones con interfaz gráfica como [Git Cola](https://git-cola.github.io/) o similares desde Deepin Store.

## Qué es Jekyll

Para que cada publicación en *Deepin en Español* sea rápida, colaborativa y segura, tenemos que desarrollar un mecanismo. Ese mecanismo para elaborar la página web y los contenidos se llama [Jekyll](https://jekyllrb.com/).

Jekyll es similar a Wordpress, Joomla o Blogger. La ventaja es, que al ser de código abierto, su facilidad de uso tipo rompecabezas. El requisito principal es un servidor que permita ejecutar archivos escritos en [Ruby](https://es.wikipedia.org/wiki/Ruby).

## Carpetas y actualizaciones
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
* Play Video and Audio with [Mediaelement.js]({{ site.url }}/info/mediaelement/)

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

La fuente oficial de Git proviene del [manual de 2014](https://git-scm.com/book/es/v2).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
