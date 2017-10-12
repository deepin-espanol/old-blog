---
layout: page-fullwidth
title: "Jekyll"
subheadline: "Ayuda"
teaser: "Aprendiendo de Git y Jekyll, ¿qué son?"
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
{% include alert text='Actualizado el 31 de julio de 2017. Es posible que sufran algunos cambios para casos específicos.' %}

## Qué es Jekyll

Para que cada publicación en *Deepin en Español* sea rápida, colaborativa y segura, tenemos que desarrollar un mecanismo. Ese mecanismo para elaborar la página web y los contenidos se llama [Jekyll](https://jekyllrb.com/).

Jekyll te permite hacer blogs como en Wordpress, Joomla o Blogger. La diferencia es la estructura tipo rompecabezas entre carpetas y archivos (que cabe menos de 3 MB sin contenido). El requisito principal es un servidor que permita ejecutar archivos escritos en [Ruby](https://es.wikipedia.org/wiki/Ruby).

La última versión de Jekyll es 3.0.

## Carpetas y actualizaciones
En caso que quieras actualizar Feeling Responsive tendrás que tomar en cuenta:

* La configuración propia como la carpeta " _data" y el archivo " _config.yml", esos no se modifican;
* Los archivos para que el servidor interprete código como "Gemfile", se puede modificar si fuera necesario;
* Las carpetas base como " _includes" para HTML, " _layouts" para traducir los posts, " _sass" para el framework Foundation si se deben actualizar;
* La carpeta "assets" para las liberías Javascript y CSS requiere atención, exepcto "img" que posee los iconos propios y no se deben perder

### Porqué usamos Jekyll

Publicaciones:
* Incrusta galería, vídeos y tipografía en las publicaciones
* Publicaciones con imagen de fondo
* Posts fáciles de hacer con Markdown
* Categorías y etiquetas como "noticias" y otros
* Reproduce contenido multimedia con [Mediaelement.js]({{ site.url }}/tutopost/mediaelement/)

CMS:
* Similar a las páginas web estáticas
* Compatible con GitHub Pages
* Navegación, encabezado y pie de página editable
* Traducible a otros idiomas (no en nuestro caso)
* Pesa menos de 3 MB de código fuente, siendo práctico de actualizar
* Fácil de instalar con config.yml en lugar de largos asistentes

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

Citamos al vídeo de [Codecourse](https://www.youtube.com/watch?v=iWowJBRMtpc) acerca de Jekyll.s

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
