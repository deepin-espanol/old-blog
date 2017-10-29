---
layout: page-fullwidth
title: "Sección para tutoriales"
subheadline: "Tutopost"
teaser: "Colaboradores en acción"
permalink: "/tutopost/"
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
{% include alert text='Actualizado el 25 de setiembre de 2017. Es posible que sufran algunos cambios para casos específicos.' %}

Bienvenidos a Tutopost, ¡el taller de la comunidad! Esta selección está pensado en crear, organizar y mejorar publicaciones (o posts) y materiales para Deepin en Español. Contiene una serie de tutoriales hacia los nuevos colaboradores a experimentados.

## Para usuarios de Wordpress y Blogger
¿Quieres añadir un post a la página web? Si eres usuario Wordpress o Blogger te costará un poco entender la interfaz de usuario. El mejor consejo es usar el cliente Atom, fácil de usar, organizada e intuitiva. La otra opción es mediante su sitio web.

Las páginas están escritas en Markdown. Nosotros usamos Git para sincronizar los cambios de los editores y gestionamos los permisos en esa plataforma.

## Tutoriales
<div class="row t60">
    <div class="medium-6 columns b30">
      Formas de editar la página web y añadir post:
      <ul>
       <li><a href="{{ site.url }}{{ site.baseurl }}/tecnico/desdeatom/">Desde Atom</a>.</li>
       <li> <a href="{{ site.url }}{{ site.baseurl }}/tecnico/usargithub/">Desde la web de Github</a>.</li>
      </ul>
      Qué contiene el post:
      <ul>
      <li> <a href="{{ site.url }}{{ site.baseurl }}/tecnico/encabezadopost/">Encabezado post</a>.</li>
      <li> <a href="{{ site.url }}{{ site.baseurl }}/tecnico/cuerpopost/">Cuerpo del post</a>.
      </ul>
    </div><!-- /.medium-6.columns -->

    <div class="medium-6 columns b30">
    <ul>
        <h3>Lista completa</h3>
        {% for post in site.tags.tutopost %}
        <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
    </ul>
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->

## Agradecimientos

Este editor fue creado para Deepin en Español y está licenciado bajo MIT.

La fuente oficial de Git proviene del [manual de 2014](https://git-scm.com/book/es/v2).

Algunos tutoriales sobre Markdown lo encontrarás [Commonmark.org](http://commonmark.org/help/tutorial/) (en inglés)

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
