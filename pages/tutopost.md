---
layout: page-fullwidth
title: "Sección para tutoriales"
subheadline: "Tutopost"
teaser: "Colaboradores en acción"
permalink: "/info/tutopost/"
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

Bienvenidos a tutopost. Esta secc

## En esta categoría:

<ul>
    {% for post in site.categories.tutopost %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

La fuente oficial de Git proviene del [manual de 2014](https://git-scm.com/book/es/v2).

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
