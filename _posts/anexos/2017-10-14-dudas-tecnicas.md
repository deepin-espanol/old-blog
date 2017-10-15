---
layout: page-fullwidth
title: "Dudas técnicas sobre Deepin"
teaser: "Para que los especialistas conozcan a detalle"
categories:
    - anexos
tags:
    - dudas
    - comunidad
header:
   image_fullwidth: "hot.jpg"
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
{% include _improve_content.html %}

En la *Comunidad Deepin* aclaramos que el sistema operativo  perfecto no existe. Buscamos que cualquiera conozca Deepin, como si fuera un vehículo o una ciudad.

En esta página respondemos las dudas más profundas. Está dedicada a personas que buscan conocer el mecanismo de dicho software.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Como distribución Linux
### ¿Qué es GNU/Linux? ¿Porqué GNU?
En realidad GNU es un proyecto desarrollado por Richard M. Stallman y fue el pilar para el desarrollo del sistema operativo. Anteriormente el señor Stallman desarollaba versiones propias hasta que...

>Empezamos a desarrollar GNU en 1984, años antes de que Linus Torvalds comenzase a escribir su núcleo. Nuestro objetivo era desarrollar un sistema operativo libre completo. [...] Desarrollamos la mayoría de los componentes principales, conformando la contribución más grande de todo el sistema.

Fuente: [FSF](https://www.gnu.org/gnu/gnu-linux-faq.es.html#why)

### ¿Deepin esta basado en Ubuntu?
Hasta las versión 2014, estuvo basado en Ubuntu. En la versión 15.x se cambió.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Deepin está basado en Debian?
Sí, para ganar estabilidad (
[Muy Linux](http://www.muylinux.com/2015/12/31/deepin-15/)).

Si no te gusta la base Debian, prueba la versión Manjaro Deepin, hecha por la comunidad. [Revisa la página Instalación]({{ site.url }}/instalacion/).
<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="Paisaje">

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Deepin tiene el sistema de apago SystemD?
Sí.

### ¿Deepin usa un núcleo Linux puro o modificado?
Modificado basado en una versión a largo plazo (LTS). Revisa el [código fuente]({{ site.url }}{{ site.baseurl }}/source) y las actividades que [puedes colaborar]({{ site.url }}{{ site.baseurl }}/actividades/kernel/).

Si tienes problemas con el núcleo, visita [la página para cambiar el núcleo de Linux]({{ site.url }}{{ site.baseurl }}/tips/kernel/).
<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="Paisaje">

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo conseguir un controlador de gráficos desarrollado por la empresa?
Sí. Algunos paquetes para optimizar la tarjeta gráfica de NVidia, por ejemplo, está disponible por separado. Visita [está página para conocer los controladores exclusivos disponibles]({{ site.url }}/manual/videocard/).

## Cómo sistema operativo único
### ¿Deepin es capaz de ejecutar videojuegos?
Sí. Echa un vistazo en [Juegos para Deepin]({{ site.url }}{{ site.baseurl }}/games/). Lo puedes conseguir en la Deepin Store, Steam o con ayuda de [Crossover]({{ site.url }}{{ site.baseurl }}/apps/crossover/).

Adicionalmente tendrás que modificiar parte del código para optimizar el sistema operativo, como este vídeo.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/CnSkR96iIpY" frameborder="0" allowfullscreen></iframe>
</div>

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Existen pruebas de que Deepin te espía?
No. El sistema operativo, al ser de [código abierto]({{ site.url }}{{ site.baseurl }}/source/), se audita por la comunidad.

Sin embargo, usamos plugins para facilitar el uso con los servicios de la nube. Por ejemplo: reconocer la letra de la canción gracias a Netease, comprobar actualizaciones, enviar el registro de error al Feedback de Deepin, etcétera.

La mayoría de paquetes incluídos en Deepin son elaboradas junto a la comunidad de Debian. Pero, el resto de aplicaciones preinstaladas, en convenio con otras empresas, aplican otras condiciones de uso.

Fuente: [Distros da China - Deepin espiona usuários?](https://www.youtube.com/watch?v=utW1J4hEJhI), [Deepin.org](https://web.archive.org/web/20170703051201/https://www.deepin.org/cooperative/netease-cloud-music/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo hace Deepin seguro?
Cada actualización es [señalada en la página web](https://www.deepin.org/en/security-update/). El núcleo del sistema [está siendo auditado frecuentemente](https://lamiradadelreplicante.com/2017/09/01/agencia-alemana-de-ciberseguridad-el-generador-de-numeros-aleatorios-de-linux-es-seguro/).

## Seguimos creciendo

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
