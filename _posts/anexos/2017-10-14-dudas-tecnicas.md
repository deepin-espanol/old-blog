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

En esta página respondemos las dudas más profundas. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/). Está dedicada a personas que buscan conocer el mecanismo de dicho software.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Como distribución Linux
### ¿Qué es GNU/Linux? ¿Porqué ambos?
En realidad GNU es un proyecto desarrollado por Richard M. Stallman y fue el pilar para el desarrollo del sistema operativo. Anteriormente el señor Stallman desarollaba versiones propias hasta que...

>Empezamos a desarrollar GNU en 1984, años antes de que Linus Torvalds comenzase a escribir su núcleo. Nuestro objetivo era desarrollar un sistema operativo libre completo. [...] Desarrollamos la mayoría de los componentes principales, conformando la contribución más grande de todo el sistema.

Fuente: [FSF](https://www.gnu.org/gnu/gnu-linux-faq.es.html#why)

### ¿En qué está basado Deepin?
En la distribución madre Debian. Específicamente la rama Sid.

Hasta las versión 2014 estuvo basado en Ubuntu. En la versión 15.x se cambió a Debian para ganar estabilidad (
[Muy Linux](http://www.muylinux.com/2015/12/31/deepin-15/)).

### ¿Puedo usar Manjaro en lugar de Debian?
Si tienes dificultades con la base Debian, prueba la versión Manjaro Deepin. [Revisa la página Instalación]({{ site.url }}/instalacion/). Recuerda que no está siendo desarrollado oficialmente, sino por la comunidad.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo se funciona el sistema de encendido y apagado en Deepin?
Deepin tiene un programa de apagado llamado [systemd](https://en.wikipedia.org/wiki/Systemd). Este "demonio" permite comprobar los dispositivos activados durante su encendido. Así, indica que está funcionando y avisa si encuentra algún error.

### ¿Deepin usa un núcleo Linux puro o modificado?
Modificado basado en una versión a largo plazo (LTS). Revisa el [código fuente]({{ site.url }}{{ site.baseurl }}/source) y las actividades que [puedes colaborar]({{ site.url }}{{ site.baseurl }}/actividades/kernel/).

Si tienes problemas con el núcleo, visita [la página para cambiar el núcleo de Linux]({{ site.url }}{{ site.baseurl }}/tips/kernel/).
<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="Paisaje">

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo conseguir un controlador de gráficos desarrollado por la empresa?
Sí. Algunos paquetes para optimizar la tarjeta gráfica de NVidia, por ejemplo, está disponible por separado. Visita [está página para conocer los controladores exclusivos disponibles]({{ site.url }}/manual/videocard/).

<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="Paisaje">

### ¿Por qué me aparece el aviso "conflicto de dependencias"?
El "conflicto de dependencias" resulta tedioso para actualizar los controladores o instalar aplicaciones. Si un programa requiere una libería en desarrollo, no podrás instalar. Si cambias la libería, podrías

]({{ site.url }}{{ site.baseurl }}manual/instalar-apps/)

Para evitar ese tipo de problemas, sugerimos instalar y actualizar aplicaciones via Deepin Store o PPA. Desde Deepin 15.5, puedes instalar via Flatpak para que disfrutes de la última versión de tus aplicaciones sin contratiempos.

Fuente: [Manual de Debian](https://www.debian.org/doc/manuals/aptitude/ch02s03s02.es.html)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Cómo sistema operativo único
### ¿Deepin es capaz de ejecutar videojuegos?
Sí. Echa un vistazo en [Juegos para Deepin]({{ site.url }}{{ site.baseurl }}/games/). Lo puedes conseguir en la Deepin Store, Steam o con ayuda de [Crossover]({{ site.url }}{{ site.baseurl }}/apps/crossover/).

Adicionalmente tendrás que modificiar parte del código para optimizar el sistema operativo, como este vídeo.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/CnSkR96iIpY" frameborder="0" allowfullscreen></iframe>
</div>

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Deepin envía los datos guardados a desconocidos?
No. El sistema operativo no envía datos a desconocidos. Al ser de [código abierto]({{ site.url }}{{ site.baseurl }}/source/), puedes comprobar por tu cuenta.

Sin embargo, usamos plugins para facilitar el uso con los servicios de la nube. Por ejemplo: reconocer la letra de la canción gracias a Netease, comprobar actualizaciones, enviar el registro de error al Feedback de Deepin, etcétera.

La mayoría de paquetes incluídos en Deepin son elaboradas junto a la comunidad de Debian. Pero, el resto de aplicaciones preinstaladas, en convenio con otras empresas, aplican otras condiciones de uso.

Fuente: [Distros da China - Deepin espiona usuários?](https://www.youtube.com/watch?v=utW1J4hEJhI), [Deepin.org](https://web.archive.org/web/20170703051201/https://www.deepin.org/cooperative/netease-cloud-music/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo podemos saber las útlimas actualizaciones de seguridad?
Cada actualización es [señalada en la página web](https://www.deepin.org/en/security-update/). El núcleo del sistema [está siendo auditado frecuentemente](https://lamiradadelreplicante.com/2017/09/01/agencia-alemana-de-ciberseguridad-el-generador-de-numeros-aleatorios-de-linux-es-seguro/).

## Seguimos creciendo

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
