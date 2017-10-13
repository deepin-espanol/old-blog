---
layout: page-fullwidth
title: "Cómo hacemos los posts"
subheadline: "Ayuda"
teaser: "Un vistazo para hacer artículos para principianes"
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
{% include alert text='Actualizado el 12 de octubre de 2017. Es posible que sufran algunos cambios para casos específicos.' %}

## Qué es git y Jekyll

Los detalles puedes encontrar en [esta página]({{ site.url }}{{ site.baseurl }}/tecnico/git/).

## Usar Atom

Este es la forma más sencilla de elaborar un post. Tienes integrado el editor de texto, la vista de carpetas y el mencionado cliente. Los detalles encotrarás [en esta página]({{ site.url }}{{ site.baseurl }}/tecnico/desdeatom/)

## Información adicional

Para empezar, como explicamos anteriormente, puedes usar un cliente como [Atom]({{ site.url }}{{ site.baseurl }}/tecnico/git/), [Gitcola](https://git-cola.github.io/) o Gitkraken desde la Deepin Store.

Si usas [la página web de Github]({{ site.url }}{{ site.baseurl }}/tecnico/usargithub/), el mecanismo se hace más gráfico.

### Clona

Abre el cliente, en este caso Importa el fichero `.git` desde https://github.com/deepin-espanol/deepin-espanol.github.io.git

En el caso de la terminal:

~~~
git clone https://github.com/deepin-espanol/deepin-espanol.github.io.git
~~~

### Carpetas

Como no hay interfaz web, desde tu gestor de archivos en el lugar:

* Las carpetas para páginas como " _drafts" para borradores, " _posts" para publicaciones en el blog y "pages" para páginas especiales; y
* La carpeta para las imágenes como "images".

### Borradores a post

1. Busca la carpeta * > _draft > ejemplo
2. Selecciona un archivo. Más detalles en la siguiente sección.
3. Pega a la carpeta * >_draft > mejorar
4. Realiza los retoques, comprueba si el código funciona correctamente.
5. Corta el archivo
6. Muévelo a post > [carpeta]. Siendo carpeta, el manual, blog o tips.

### Encabezado del post

Cuando creas un archivo asegúrate que contenga:

* title: "" (título)
* subheadline: "" (subtítulo)
* teaser: "" (adelanto)
* categories: (como manual, blog, app o tip)
* tags: (etiqueta)

Más detalles en ["Planilla del post"]({{ site.url }}/tecnico/plantillapost/).

### Cuerpo del post y Markdown

El lenguaje que aplicamos es [Markdown](https://es.wikipedia.org/wiki/Markdown) por ser fácil de aprender, casi lo mismo a una wiki.

* Escribe `*cursiva*` sale *cursiva*
* Escribe `**negrita**` sale **negrita**
* Escribe  `[Texto del enlace aquí](URL "Título del enlace")` y creas un enlace
* Escribe `![Texto alternativo](URL "Título de la imagen")` y creas una imagen

Para aprender todas las posibilidades visita [Códigos permitidos en Markdown]({{ site.url }}/tecnico/doc/). Si quieres editar desde la web, te presentamos [JBT](https://jbt.github.io/markdown-editor/) o [Diliger](http://dillinger.io/).

## Ramas, subida y bajada de parches

Pare realizar un commit o parche, asegúrate que hayas realizado modificaciones como los nuevos archivos que has creado.

Primero: Una vez realizado el parche tienes dos opciones:

8. Haz un push en la branch o rama "[usuario]-post".
9. Si deseas pueds añadir más parches para corregir algunos percances.
10. Cuando está listo, tendrás que hacer la orden "push" a la rama "master".
11. Si hay conflictos por aplicar paches antes de tiempo, es mejor realizar un "fetch" de la rama que vas a aplicar.

### Opcional: Crea una rama

Si deseas puedes crear una rama para evitar conflictos de edición. Desde git-cola crea una nueva rama.

9. Dale un nombre la rama "merge"
10. Hacer un "merge" en la rama "master".

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Opcional: Hacer un "pullrequest"

En la web de Github (necesitas iniciar sesión) puedes hacer una solicitud para trasferir los cambios de tu rama a la "master:

10. Pide un "pull request", o solicitud para aplicar los parches, a la rama central.
11. Una vez revisado en la sección Issues, se aplican los parches y se elimina la rama obsoleta.

### Nota: Subir imágenes al sitio web

Este portal te permite subir imágenes a partir de la carpeta "images". Recomandamos comprimir lo máximo posible para que el navegador cargue más rápido y no desperdicie ancho de banda

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

La fuente oficial de Git proviene del [manual de 2014](https://git-scm.com/book/es/v2).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
