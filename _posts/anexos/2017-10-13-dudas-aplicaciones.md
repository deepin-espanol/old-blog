---
layout: page-fullwidth
title: "Dudas más frecuentes sobre las aplicaciones"
teaser: "Ayudando a que las aplicaciones funcionen"
categories:
    - anexos
tags:
    - dudas
    - comunidad
    - guiapps
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

En esta página respondemos las dudas más comunes relacionadas al funcionamiento de las aplicaciones y algunos incovenientes. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## General
### ¿Qué juegos puedo instalar?
En teoría, puedes correr cualquier [juego diseñado para Linux]({{ site.url }}{{ site.baseurl }}/manual/juegos).

En caso que prefieras instalar juegos con ejecutables para Microsoft Windows, incluyendo al componente DirectX, tendrás que usar Wine ([PlayonLinux]({{ site.url }}{{ site.baseurl }}/tips/playonlinuxapps) o [Crossover]({{ site.url }}{{ site.baseurl }}/manual/exeapps/)). Consigue el ejecutable desde el disco o la carpeta de instalación y sigue las instrucciones.

No olvides tener tu catálogo local con [Lutris]({{ site.url }}{{ site.baseurl }}/apps/lutris/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo reporto un error en Deepin?
Siempre que estén disponibles en la tienda Deepin Store, reporta fallas gráficas, problemas de rendimiento o arranque a [Deepin Feedback]({{ site.url }}{{ site.baseurl }}/actividades/feedback) (también llamado Comentarios de Deepin).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Instalación
### ¿Puedo instalar aplicaciones sin necesidad de Deepin Store?
Sí. En otra distribuciones, la forma más segura es usando la aplicación [Synaptic]({{ site.url }}{{ site.baseurl }}/apps/synaptic/) e instalando los paquetes que necesites desde sus repositorios.

También puedes instalar desde sitios web. Antes de proceder a ese método, comprueba el [tipo de instalación]({{ site.url }}{{ site.baseurl }}/manual/instalar-apps/) o sigue leyendo.

### ¿Qué es el aviso "conflicto de dependencias" y porque desaconsejamos instalar por paquetes deb?
El "conflicto de dependencias" resulta tedioso para actualizar los controladores o instalar aplicaciones mediante paquetes de Debian. Ocurre al instalar dependencias que alteran el funcionamiento normal como los paquetes Mesa, Qt, códecs, entre otros.

Para evitar ese tipo de problemas, sugerimos instalar y actualizar aplicaciones via [Deepin Store]({{ site.url }}{{ site.baseurl }}manual/instalar-apps/) o PPA.

Fuente: [Manual de Debian](https://www.debian.org/doc/manuals/aptitude/ch02s03s02.es.html)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Por qué recomendamos Flatpak o Snap?
Puedes instalar y utilizar aplicaciones sin problemas. Sus componentes se actualizan de forma silenciosa y no interfieren con los componentes del sistema. Flatpak es desarrollado por la comunidad y Snap por Cannonical.

Por su puesto, las aplicaciones originales están integradas bajo Flatpak. Disponibles desde la versión 15.5 del sistema operativo. Si quieres conocer este método de instalación visita [flatpak.org](http://flatpak.org/apps.html).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Aplicaciones pesadas

### ¿Puedo instalar Photoshop?
Hasta que Adobe se dedique a explorar otras formas, puedes usar la versión web de Photoshop o usar su versión para Android [Photoshop Fix](https://play.google.com/store/apps/details?id=com.adobe.adobephotoshopfix), requiere [Genymotion]({{ site.url }}{{ site.baseurl }}/apps/genymotion/) o [similares]({{ site.url }}{{ site.baseurl }}/anexos/guiapps/).

[Gimp]({{ site.url }}{{ site.baseurl }}/apps/gimp/), disponible en Deepin Store, tiene funcionalidades interesantes. Si lo usas, tienes la oportunidad de personalizar su interfaz.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo instalar AutoCad?
Hasta el 2017, no todas las versiones funcionan con éxito, las más recientes no permiten instalar. Visita [esta lista de alternativas]({{ site.url }}{{ site.baseurl }}/anexos/appsprofesion/)

Fuente: [Wine](https://appdb.winehq.org/appview.php?iAppId=86), [Foro de AutoDesk](https://web.archive.org/web/20171014134437/https://forums.autodesk.com/t5/autocad-forum/autocad-support-for-linux-becoming-a-major-management-decision/td-p/3051192/page/10?nobounce), [Hipertextual](https://web.archive.org/web/20160603181746/http://hipertextual.com:80/2013/09/alternativas-libres-autocad)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Seguimos creciendo

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
